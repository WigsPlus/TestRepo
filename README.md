# Hospital README

# Postman

Getting a doctor which is autherrized for a patient on a adsission:

http://localhost:5000/api/Admissions/67048766/0   // Changing the "0" to "1" will give a no perssin since that doctor is not autorized to taht patient

Getting all doctors:

http://localhost:5000/api/Doctors

Getting a single doctor by ID:

http://localhost:5000/api/doctors/doctorId=0

Creating a doctor with a JSON body:

http://localhost:5000/api/doctors/

{
    "doctorId": 5,
    "name": "Jørgen",
    "department": "Århus"
}


# Docker Setup

In terminal for setup:(Proberly not needed)

docker build -t wiggersdocker/hospital .

Running the container from the dockerhub:

docker run -p 8080:5000 wiggersdocker/hospital 
