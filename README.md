# mega
good


پیش نیاز های سورس:

 sudo apt-get update; sudo apt-get upgrade; sudo apt-get install tmux; sudo apt-get install luarocks; sudo apt-get install screen; sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev lua-socket lua-sec lua-expat libevent-dev make unzip git redis-server autoconf g++ libjansson-dev libpython-dev expat libexpat1-dev; sudo apt-get update; sudo apt-get install; sudo apt-get install upstart-sysv

جدا از هم

 wget http://luarocks.org/releases/luarocks-2.2.2.tar.gz;tar zxpf luarocks-2.2.2.tar.gz;cd luarocks-2.2.2 && ./configure; sudo make bootstrap;sudo luarocks install luasocket;sudo luarocks install luasec;sudo luarocks install redis-lua;sudo luarocks install lua-term;sudo luarocks install serpent;sudo luarocks install dkjson;sudo luarocks install lanes;sudo luarocks install Lua-cURL

بعد کد :
 cd
======================
  پوشه سورس رو اپلود کن داخل سرور
======================
3️⃣ وارد شماره‌ ربات شو و  یه ربات (api) با
 @Botfather
بساز اسم و ایدی وارد کن (بعد باید اینلاین را فعال کنی
 
وارد مسیر زیر شو:

MaTaDoR/api/bot/bot.lua

 خط [3] توکن ربات (api)
 خط [5] ایدی سودو
خط [165] ایدی سودو و ایدی ربات cli
سیو کن خارج شو ....

 وارد مسیر زیر شو

MaTaDoR/cli/bot/bot.lua

خط [18] ایدی ربات (api) را وارد ایدی اول توکن هست.
خط 75  ایدی سودو و ایدی ربات cli
سیو کن خارج شو....

وارد مسیر زیر شو

MaTaDoR/cli/data/config

چندتا ایدی هس اولی ایدی سودو دومی ایدی ربات cli بقیشو بپاک بعد سیو کن.

وارد مسیر زیر شو

MaTaDoR/cli/Plugins

فایل mrcore.lua روباز کن
 خط ۱ ایدی عددی سودو رو بزار

 دستورات زیر در ترمینال بزن کپی کن پیست کن بعد اینتر ...
 

cd MaTaDoR/cli && chmod +x matador.sh && chmod 777 auto.sh && sed -i -e 's/\r$//' auto.sh && ./matador.sh install
کامل نصب شد کد زیر
 

 ./matador.sh
شماره ربات وارد کن.

از سرور خارج و دوباره وصل شو

کد های زیر را در سرور میزنیم
 

cd MaTaDoR/api && chmod +x matador.sh && chmod 777 auto.sh && sed -i -e 's/\r$//' auto.sh && ./matador.sh install
کامل نصب شد بعد کد :
 

 ./matador.sh
تمام حالا باید لانچ کنی ولی قبلش 👇

 قبل از لانچ شدن ربات (api) همون هلپر باید هم با اکانت ربات هم با اکانت سودو ربات هلپر رو /start بزنی.

حالا لانچ کن :
 

cd MaTaDoR/api && chmod +x auto.sh && chmod 777 auto.sh && screen ./auto.sh
یه ترمینال دیگه باز کن و کد :
 

cd MaTaDoR/cli && chmod +x auto.sh && chmod 777 auto.sh && screen ./auto.sh
