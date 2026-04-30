## Jojo's Hospital: A Ransomware Investigation  

A ransomware group named "LockByte" has stolen and encrypted files a hospital has. They are demanding a ransom of $2 million dollars within 72 hours. If not met, they will leak the sensitive information publicly. The hackers have asked the patients to pay $10,000 dollars. 

### General Notes 

- 6420 files were encrypted. They are 321 unique hostnames that had encrypted files on them. 

- The ransom file is "We_Have_Your_Data_Pay_Up.txt". The sha256 hash on the file is 97c348e95c8a8aeb8808f76434d73a92bbcb6b4586788365762b22624990b018. 
    - The path to this file is "C:\Users\andavis\Documents\We_Have_Your_Data_Pay_Up.txt". Only one device had this: hostname = AMFB-MACHINE, username = andavis. 
    - The actual employee is "Anthony Davis", his IP is 10.10.0.1, his email is anthony_davis@jojoshospital.org. 

- The group used "patient_data_exporter.exe" to steal data from the hospital and specifically took patient records, archived patient records and old patient data; put into 3 zip files. They then sent the data to a domain called "secure-health-access.com". 