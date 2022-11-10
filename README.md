# Secure-File-Storage-In-Cloud-Using-Hybrid-Cryptography

Storing the file on the secure platform

# STEPS:

ENCRYPTION</br>
1. Upload a <i>text-file</i> on the server</br>
2. Download the public-key (.pem)</br>

DECRYPTION</br>
1. Upload public-key on the server</br>
2. Download the decrypted file</br>

# METHODOLOGY:

To secure the file:
1. Uploading of file on the server.</br>
2. Dividing the uploaded file into N-equal-parts (33kb each) and stored in "files" folder.</br>
3. Encrypting all the parts of the file using any 1 of the 4 algorithms and stored in "encrypted" folder.</br>
(Algorithm is changed with every part in round-robin-fashion)</br>
4. Public-key will be generated and hence the file is secured.</br>

To restore the file:</br>
1. Load the public-key on the server.</br>
2. Decryption of the public-key.</br>
3. All the N parts are now processed for decryption using the same algorithms which were used to encrypt them.</br>
4. Combine all the N parts to form the original file and provide it to the user for downloading.</br>

# HOW TO RUN:

Step 1: Install Requirements</br>
`pip install -r requirements.txt`</br>

Step 2: Run the application</br>
`python app.py`</br>

Step 3: Visit the localhost from your browser</br>
`eg. http://localhost:port`

Have Fun!👨‍💻</br>
Enjoy🙂💖
