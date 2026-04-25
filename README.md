

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
<img width="1024" height="773" alt="Screenshot 2026-04-24 215239" src="https://github.com/user-attachments/assets/ea24cb89-1c2a-48b2-9c39-b7243caa5fe4" />
<img width="1022" height="770" alt="Screenshot 2026-04-24 215250" src="https://github.com/user-attachments/assets/e5c8cc10-d3ea-4890-a71e-4825af9d9fdf" />
<img width="1019" height="772" alt="Screenshot 2026-04-24 215300" src="https://github.com/user-attachments/assets/a18a57b6-3a41-4154-bbc1-736e536288fa" />
<img width="1022" height="771" alt="Screenshot 2026-04-24 215315" src="https://github.com/user-attachments/assets/c77e1b8a-4843-4ce2-9630-ed378faa8e84" />

Після встановлення необхідних служб необхідно сконфігорувати наш домен. Іменем нашого домену буде my.domain
<img width="1020" height="771" alt="Screenshot 2026-04-24 215555" src="https://github.com/user-attachments/assets/368989fb-1fcf-42b5-9571-ec76a7881a61" />
<img width="1023" height="772" alt="Screenshot 2026-04-24 215639" src="https://github.com/user-attachments/assets/bc8a40d7-9937-4753-92f6-1b97b4d03ce6" />
<img width="1020" height="768" alt="Screenshot 2026-04-24 215709" src="https://github.com/user-attachments/assets/387e4350-d3fb-422e-82f5-098458762ebd" />
<img width="1022" height="769" alt="Screenshot 2026-04-24 215733" src="https://github.com/user-attachments/assets/e6eed8b9-6f5d-4fdb-bac9-53d4711642c8" />
<img width="1022" height="772" alt="Screenshot 2026-04-24 215757" src="https://github.com/user-attachments/assets/8c319483-c091-4599-aa47-b22fac3041d6" />
<img width="1020" height="767" alt="Screenshot 2026-04-24 215818" src="https://github.com/user-attachments/assets/fbd7a74d-d4c0-41dc-8c21-0929be720be5" />
<img width="1022" height="767" alt="Screenshot 2026-04-24 215834" src="https://github.com/user-attachments/assets/7cef8ba6-6449-419e-91d1-3e76bf18f79a" />
<img width="1021" height="771" alt="Screenshot 2026-04-24 215855" src="https://github.com/user-attachments/assets/64432547-485f-4ab2-a42d-e5daedfab05d" />

Після встановлення служб і перезавантаження системи, бачимо що вхід здійснюється вже в домені
<img width="1015" height="755" alt="Screenshot 2026-04-24 220345" src="https://github.com/user-attachments/assets/6de58866-cd34-4f57-b417-bd25dbc8610b" />

Після входу додаємо акаунт користувача в домені (user1) як показано на слайдах
<img width="1020" height="774" alt="Screenshot 2026-04-24 220455" src="https://github.com/user-attachments/assets/a4c3fb4c-965e-409c-87b5-eae3e6252695" />
<img width="1018" height="771" alt="Screenshot 2026-04-24 220529" src="https://github.com/user-attachments/assets/7992e230-90a7-43d6-b1b7-86991362f980" />
<img width="1020" height="770" alt="Screenshot 2026-04-24 220605" src="https://github.com/user-attachments/assets/876bed22-247d-4f3d-bc26-b19b0ede0d56" />
<img width="1015" height="769" alt="Screenshot 2026-04-24 220635" src="https://github.com/user-attachments/assets/62b2efdc-c16c-4a7f-9068-1b611e12573f" />

Бачимо що профіль користувача успішно створений
<img width="1021" height="765" alt="Screenshot 2026-04-24 220649" src="https://github.com/user-attachments/assets/db0c6a93-d11c-4324-96e2-b91537be4b39" />

2. Створення віртуальної машини кліента
   Для віртуальної машини клієнта будемо використовувати образ Windows 11
   Параметри віртуальної машини можна використати такі самі як і на сервер
   <img width="1272" height="746" alt="Screenshot 2026-04-24 224420" src="https://github.com/user-attachments/assets/b98f0c23-fca4-407d-a5b7-f2a230d34aff" />

Далі йде стандартна процедура встановлення системи Windows 11
<img width="1022" height="784" alt="Screenshot 2026-04-24 225641" src="https://github.com/user-attachments/assets/ddb0d762-506b-4521-9eab-4451ccf2d924" />
<img width="1021" height="785" alt="Screenshot 2026-04-24 225709" src="https://github.com/user-attachments/assets/e0d566c8-81ca-4e85-89f9-56f09353d006" />
<img width="1018" height="783" alt="Screenshot 2026-04-24 225732" src="https://github.com/user-attachments/assets/8a1875ca-15ab-4c67-b52c-87cb16abf6e5" />
<img width="1021" height="787" alt="Screenshot 2026-04-24 225750" src="https://github.com/user-attachments/assets/199fa217-0da7-41a1-aa67-21991f61edfc" />
<img width="1019" height="783" alt="Screenshot 2026-04-24 225802" src="https://github.com/user-attachments/assets/ce490c2f-fb46-4331-8366-c2cc9cdfce4d" />
<img width="1019" height="785" alt="Screenshot 2026-04-24 225908" src="https://github.com/user-attachments/assets/4ab47d36-fb10-46e4-b4af-6b30a8cb2551" />
<img width="1023" height="789" alt="Screenshot 2026-04-24 225928" src="https://github.com/user-attachments/assets/f63c4c98-fb2f-4f1c-8b1d-2f3f84a71903" />

<img width="1022" height="785" alt="Screenshot 2026-04-24 231803" src="https://github.com/user-attachments/assets/5b85804a-c9d9-4de3-b8f7-1efbbc89ae56" />
<img width="1021" height="787" alt="Screenshot 2026-04-24 231828" src="https://github.com/user-attachments/assets/bee7c4f9-a278-4d00-9dad-9dab68f79587" />
<img width="1022" height="788" alt="Screenshot 2026-04-24 231835" src="https://github.com/user-attachments/assets/ade7f321-a595-4ed7-837e-5d49cc9673ae" />
<img width="1022" height="788" alt="Screenshot 2026-04-24 232008" src="https://github.com/user-attachments/assets/ca1244eb-bbb1-4cd3-a090-2a585229dcf3" />

<img width="1023" height="790" alt="Screenshot 2026-04-24 232018" src="https://github.com/user-attachments/assets/6e1dcfde-b919-4aa4-83a7-529d031bc039" />
<img width="1023" height="786" alt="Screenshot 2026-04-24 232301" src="https://github.com/user-attachments/assets/48159010-1cdb-4c17-b64b-c64ea85143e3" />

Після завершення встановлення, заходимо в систему.
Для того щоб наш клієнт успішно доєднався до домену, вони мають бути в одній мережі і сервер виступав в ролі днс для клієнта, тому наступним кроком ми конфігуруємо мережу на машині клієнта

<img width="1024" height="763" alt="Screenshot 2026-04-25 152248" src="https://github.com/user-attachments/assets/b4217d15-655e-4536-af61-4053c27c45cd" />
<img width="1023" height="764" alt="Screenshot 2026-04-25 152748" src="https://github.com/user-attachments/assets/5eeaffb7-16af-444f-82b0-6bfdf0e40007" />

Перевіряємо і бачимо доступність 
<img width="1020" height="770" alt="Screenshot 2026-04-25 152410" src="https://github.com/user-attachments/assets/ad93dbcc-432f-4818-b6a0-e6d764a7243b" />

Далі додаємо машину клієнта в домен

<img width="1022" height="766" alt="Screenshot 2026-04-25 152428" src="https://github.com/user-attachments/assets/c1e746f7-cae0-4f50-aba1-aa164d0519a5" />
<img width="1022" height="769" alt="Screenshot 2026-04-25 152435" src="https://github.com/user-attachments/assets/9a49e88f-9b23-46e9-bd50-f8246582618d" />
<img width="1025" height="766" alt="Screenshot 2026-04-25 152458" src="https://github.com/user-attachments/assets/eaa0130e-a8e6-408b-bc5d-3359396d33a1" />

<img width="1024" height="768" alt="Screenshot 2026-04-25 152513" src="https://github.com/user-attachments/assets/2f46162f-15e1-4c6e-be93-8f6d634e6c46" />

<img width="1022" height="769" alt="Screenshot 2026-04-25 152541" src="https://github.com/user-attachments/assets/8445d649-38b3-42b1-a432-e9f87e854811" />

Після перезавантаження системи бачимо що логін відбувається вже в домені 

<img width="1028" height="767" alt="Screenshot 2026-04-25 152700" src="https://github.com/user-attachments/assets/6bbec3ca-5b8b-4600-bb31-c649b3995f25" />
<img width="1022" height="769" alt="Screenshot 2026-04-25 152813" src="https://github.com/user-attachments/assets/c6ac2488-1321-461f-8ae8-927dcb8b6932" />

Так і на сервері можна перевірити що додалась наша віртуальна машина клієнта 
<img width="1013" height="767" alt="Screenshot 2026-04-25 152858" src="https://github.com/user-attachments/assets/24c39243-8fdb-44e9-b92b-692e8bb25fa0" />



















