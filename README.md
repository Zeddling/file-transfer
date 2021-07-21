#   File Transfer Service
Endpoints:
1. Download file: <b>GET http://localhost:8080/{filename}</b>
2. Create remote file: <b>POST http://localhost:8080/{filename} -d "file contents"</b>
Returns name of the file created and saves the data in the file.
Filename is appended with a pseudo-random number to prevent file name collisions.
3. Replace content of existing remote file: <b>PUT http://localhost:8080/ -d "file contents"</b>
4. Delete file: <b>DELETE http://localhost:8080/{filename}</b>
