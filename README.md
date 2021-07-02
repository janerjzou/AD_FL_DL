# CapstoneProject_Anomaly_Detection_with_FL

## from March 2021 to June 2021

## Federated Deep Auto-encoder




### To load datasets
!pip install -U -q PyDrive
from pydrive.auth import GoogleAuth
from pydrive.drive import GoogleDrive
from google.colab import auth
from oauth2client.client import GoogleCredentials
<!--  Authenticate and create the PyDrive client. -->
auth.authenticate_user()
gauth = GoogleAuth()
gauth.credentials = GoogleCredentials.get_application_default()
drive = GoogleDrive(gauth)

id = '1M3LKek2UCf9HXEieWLDpFHN8PSh7088u'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #1.csv')   # Device #1

id = '19H5gOya_F-DQbaOxyamV9nK3RuSjCgK2'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #2.csv')   # Device #2

id = '1lEd9Qq3q5vy9p4VQpWCGFcuxkrdq-9l6'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #3.csv')   # Device #3

id = '1HQ3txtS2WxzJrBlIhd3GaSVHwzcQEi61'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #4.csv')   # Device #4

id = '1fmzFIkM4FhAMa73uD36j7gHtdCF9-_QV'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #5.csv')   # Device #5

id = '1zk5riI0z3tiC_4OHgTYC7oWETihs65Lj'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #6.csv')   # Device #6

id = '1rJCtnpS_XeqALJ0-CJTrCBxsQwKYlZ30'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #7.csv')   # Device #7

id = '1Mg0A0Fcelu5nsgCgfS9evve4vHGoGha6'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #8.csv')   # Device #8

id = '152_3vZEkrTRrmSs0BpMNt6CQsSnHgO82'
downloaded = drive.CreateFile({'id':id}) 
downloaded.GetContentFile('Device #9.csv')   # Device #9

<!--  add dataset links for other types of devices here..... -->




d1 = pd.read_csv('/content/Device #1.csv')
d2 = pd.read_csv('/content/Device #2.csv')
d3 = pd.read_csv('/content/Device #3.csv')
d4 = pd.read_csv('/content/Device #4.csv')
d5 = pd.read_csv('/content/Device #5.csv')
d6 = pd.read_csv('/content/Device #6.csv')
d7 = pd.read_csv('/content/Device #7.csv')
d8 = pd.read_csv('/content/Device #8.csv')
d9 = pd.read_csv('/content/Device #9.csv')
