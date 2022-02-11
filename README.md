# dsss
Fun  nv xhn
import random
import requests
import pyfiglet

Z = '\033[1;31m' #احمر
X = '\033[1;33m' #اصفر
Z1 = '\033[2;31m' #احمر ثاني
F = '\033[2;32m' #اخضر
A = '\033[2;34m'#ازرق
C = '\033[2;35m' #وردي
B = '\033[2;36m'#سمائي
Y = '\033[1;34m' #ازرق فاتح

print(Z +''' 
 ____    _    _   _ _____ ___ _____ ___  
/ ___|  / \  | \ | |_   _|_ _|_   _/ _ \ 
\___ \ / _ \ |  \| | | |  | |  | || | | |
 ___) / ___ \| |\  | | |  | |  | || |_| |
|____/_/   \_\_| \_| |_| |___| |_| \___/ 
                                         
=======================================

''')

ID = input(X+' ==> 𝙸𝙳 : ')
print('  ')
token = input(X+' ==> 𝚃𝙾𝙺𝙸𝙽 : ')
print(X+'''
 { • 𝚂𝙰𝙽𝚃𝙸𝚃𝙾 𝚃𝙾𝙾𝙻 • }
''')
H = input(X+' 𝙿𝙰𝚂𝚂 : ')

ku = ('{"account_created": false, "errors": {"email": [{"message": "Too many accounts are using a@gmail.com.", "code": "email_sharing_limit"}], "__all__": [{"message": "Create a password at least 6 characters long.", "code": "too_short_password"}]}, "dryrun_passed": false, "username_suggestions": [], "status": "ok", "error_type": "form_validation_error"}')

if H == '1':
	uus = '_6w.9u.fzqa_jcv.pnx_0517'
	
	while True:
		ks = str(''.join(random.choice(uus) for i in range(4)))
	
		url = 'https://www.instagram.com/accounts/web_create_ajax/attempt/'
	
		headers_kai={
                'accept': '*/*',
                'accept-encoding': 'gzip, deflate, br',
                'accept-language': 'ar,en-US;q=0.9,en;q=0.8,ar-SA;q=0.7',
                'content-length': '61',
                'content-type': 'application/x-www-form-urlencoded',
                'cookie': 'ig_cb=2; ig_did=BB52B198-B05A-424E-BA07-B15F3D4C3893; mid=YAlcaQALAAHzmX6nvD8dWMRVYFCO; shbid=15012; rur=PRN; shbts=1612894029.7666144; csrftoken=CPKow8myeXW9AuB3Lny0wNxx0EzoDQoI',
                'origin': 'https://www.instagram.com',
                'referer': 'https://www.instagram.com/accounts/emailsignup/',
                'sec-ch-ua': '"Google Chrome";v="87", " Not;A Brand";v="99", "Chromium";v="87"',
                'sec-ch-ua-mobile': '?0',
                'sec-fetch-dest': 'empty',
                'sec-fetch-mode': 'cors',
                'sec-fetch-site': 'same-origin',
                'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36',
                'x-csrftoken': 'CPKow8myeXW9AuB3Lny0wNxx0EzoDQoI',
                'x-ig-app-id': '936619743392459',
                'x-ig-www-claim': 'hmac.AR0Plwj5om112fwzrrYnMNjMLPnyWfFFq1tG7MCcMv5_vN9M',
                'x-instagram-ajax': '72bda6b1d047',
                'x-requested-with': 'XMLHttpRequest'

            } 
            
            
		datas_kai={
                'email' : 'a@gmail.com',
                'username': f'{ks}',
                'first_name': 'AA',
                'opt_into_one_tap': 'false'
            }
		
		kd = requests.post(url,headers=headers_kai,data=datas_kai).text
		
		if ku in kd:
			print(F + ' Y ~ ' + ks)
			
			tlg =(f'''https://api.telegram.org/bot{token}/sendMessage?chat_id={ID}&text= 
====================
NEW ⭕1
                          ×	
====================
USER : @{ks} ⭕ 4
              ×
                                             ×
BY : @KM8MM ⭕  3
         ×
====================
''')

			i = requests.post(tlg)
    
    
		else: 1

 



			print(Z + ' NOO ~ ' + ks)	
