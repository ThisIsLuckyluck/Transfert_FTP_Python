from ftplib import FTP

# Informations FTP server
ftp_host = 'Your.FTP.IP.SERVER'
ftp_user = 'Your_user'
ftp_password = 'Your_Password'


# The Path of your FTP server where you want to transfert
local_file_path = '/your/local/file/path'


# The name of your file
local_file_name = 'your_file_name'

# The path on your Server FTP
ftp_file_path = '/your/ftp/file/path'



# Create object FTP
ftp = FTP()

# Connection to the FTP server
print ("Starting Ftp")
ftp.connect(ftp_host)
print ("Connection Ftp")
ftp.login(ftp_user, ftp_password)
ftp.set_pasv(0)
ftp.cwd('/your/ftp/file/path')

print ("Ouverture Fichier")

#You path (local)

file = open('/your/local/file/path/your_file_name')  

print ("Transfert Ftp")
ftp.storbinary('STOR '+local_file_name,file)

# Closing FTP session
ftp.quit()
