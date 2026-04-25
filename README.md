# -Active-Directory

Лабораторна робота - Створення серверу Active Directory з додаванням користувача в домен
Робота виконувалась в гіпервізорі Oracle VirtualBox

1. Створення віртуальної машини серверу Active Directory
   Для віртуальної машини серверу будемо використовувати образ Windows Server 2022

Визначаємо назву серверу, а також місце створення віртуальної машини та місце розташування ташого образу серверу
   <img width="786" height="556" alt="Screenshot 2026-04-24 213003" src="https://github.com/user-attachments/assets/9f5df522-7662-45cc-93ce-3d419afb2f78" />
  Визначаємо йому наступні параметри (як показано на слайді) та зберігаємо
   <img width="1276" height="746" alt="Screenshot 2026-04-24 213609" src="https://github.com/user-attachments/assets/8f516cc1-5992-40d4-b157-e072eddf44c8" />

   Далі йде стандартне встановлення Windows, як показано в наступних слайдах

<img width="1020" height="767" alt="Screenshot 2026-04-24 213728" src="https://github.com/user-attachments/assets/ecdae340-d5f3-4e19-a6a9-b0e85a587e0b" />
<img width="1022" height="762" alt="Screenshot 2026-04-24 213755" src="https://github.com/user-attachments/assets/1e2a0d81-6ea0-4bd9-9ef5-bc5c5c989bc9" />
<img width="1022" height="766" alt="Screenshot 2026-04-24 213809" src="https://github.com/user-attachments/assets/bc7e8b7e-1b15-4860-a004-834f12c69947" />
<img width="1027" height="778" alt="Screenshot 2026-04-24 213843" src="https://github.com/user-attachments/assets/5050e321-190e-442a-8860-8a9623a9c037" />
<img width="1017" height="763" alt="Screenshot 2026-04-24 213900" src="https://github.com/user-attachments/assets/41da8c7c-50f5-4665-9bbb-bdc32347b8f6" />
<img width="1026" height="770" alt="Screenshot 2026-04-24 213911" src="https://github.com/user-attachments/assets/4718af08-d8fa-41d5-b2fa-eb14924df760" />

Визначаємо пароль адміністратора та логінимось в систему
<img width="1020" height="763" alt="Screenshot 2026-04-24 214703" src="https://github.com/user-attachments/assets/39252a43-33d7-4ccc-8a3f-70a46fd2c138" />

Для налаштування серверу для роботи з Active Directory необхідно виставити статичну ІР-адресу 
<img width="1022" height="766" alt="Screenshot 2026-04-24 215000" src="https://github.com/user-attachments/assets/ea1df10d-abed-4b21-bada-606efb3223b6" />

<img width="1019" height="769" alt="Screenshot 2026-04-24 215016" src="https://github.com/user-attachments/assets/8f509f01-efd1-4a9c-8908-a6a677b9c527" />
В нашому випадку це 192.168.10.10
<img width="1025" height="764" alt="Screenshot 2026-04-24 215044" src="https://github.com/user-attachments/assets/87459ca2-5870-4ff0-aebf-d2a509c09032" />

Далі заходимо в менеджер серверу і додаємо необхідні сервіси як показано в наступних слайдах

<img width="1023" height="769" alt="Screenshot 2026-04-24 215111" src="https://github.com/user-attachments/assets/111b6473-f5e0-4a0f-b86c-d26100e90962" />
<img width="1024" height="772" alt="Screenshot 2026-04-24 215138" src="https://github.com/user-attachments/assets/c38ea8a9-bbcc-448a-948c-b4cf62220ff2" />
<img width="1021" height="774" alt="Screenshot 2026-04-24 215149" src="https://github.com/user-attachments/assets/959e6321-2360-4a1b-b2be-7b44e25edd7a" />
<img width="1019" height="772" alt="Screenshot 2026-04-24 215200" src="https://github.com/user-attachments/assets/50cfb13b-0a2b-42ab-8674-292df697a383" />

Для успішного додавання користувачів на сервер Active Directory необхідно обов'язково додати і ДНС сервер
<img width="1023" height="766" alt="Screenshot 2026-04-24 215225" src="https://github.com/user-attachments/assets/2fc33acc-3b05-4fd8-989f-e4dc8e7bbf0b" />
































