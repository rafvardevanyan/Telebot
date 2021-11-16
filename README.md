import types

import telebot
from telebot import types

TOKEN = '2072590409:AAH7fMGWGgjRCkzm6npU1YSUyW-5eYlEuNE'
bot = telebot.TeleBot(TOKEN)


@bot.message_handler(content_types=['text'])
def get_text_message(message):
    if message.text == "Привет":
        bot.send_message(message.from_user.id, "Привет!")
    keyboard = types.InlineKeyboardMarkup()
    key_audi = types.InlineKeyboardButton(text='Audi', callback_data='audi')
    keyboard.add(key_audi)
    key_bentley = types.InlineKeyboardButton(text='Bentley', callback_data='bentley')
    keyboard.add(key_bentley)
    key_bmw = types.InlineKeyboardButton(text='BMW', callback_data='bmw')
    keyboard.add(key_bmw)
    key_cadillac = types.InlineKeyboardButton(text='Cadillac', callback_data='cadillac')
    keyboard.add(key_cadillac)
    key_ford = types.InlineKeyboardButton(text='Ford', callback_data='ford')
    keyboard.add(key_ford)
    key_honda = types.InlineKeyboardButton(text='Honda', callback_data='honda')
    keyboard.add(key_honda)
    key_hyundai = types.InlineKeyboardButton(text='Hyundai', callback_data='hyundai')
    keyboard.add(key_hyundai)
    key_landrover = types.InlineKeyboardButton(text='Land Rover', callback_data='landrover')
    keyboard.add(key_landrover)
    key_mercedesbenz = types.InlineKeyboardButton(text='Mercedes-Benz', callback_data='mercedesbenz')
    keyboard.add(key_mercedesbenz)
    key_porsche = types.InlineKeyboardButton(text='Porsche', callback_data='porsche')
    keyboard.add(key_porsche)
    key_toyota = types.InlineKeyboardButton(text='Toyota', callback_data='toyota')
    keyboard.add(key_toyota)
    key_ferrari = types.InlineKeyboardButton(text='Ferrari', callback_data='ferrari')
    keyboard.add(key_ferrari)
    key_rollsroyce = types.InlineKeyboardButton(text='Rolls-Royce', callback_data='rr')
    keyboard.add(key_rollsroyce)
    bot.send_message(message.from_user.id, text='Выбери марку!', reply_markup=keyboard)

@bot.callback_query_handler(func=lambda call: True)
def callback_worker(call):
    if call.data == "1":
        msg = 'https://auto.ru/cars/audi/a3/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "2":
        msg = 'https://auto.ru/cars/audi/a4/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "3":
        msg = 'https://auto.ru/cars/audi/a5/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "4":
        msg = 'https://auto.ru/cars/audi/a6/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "5":
        msg = 'https://auto.ru/cars/audi/a7/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "6":
        msg = 'https://auto.ru/cars/audi/a8/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "7":
        msg = 'https://auto.ru/cars/audi/q3/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "8":
        msg = 'https://auto.ru/cars/audi/q5/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "9":
        msg = 'https://auto.ru/cars/audi/q7/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "10":
        msg = 'https://auto.ru/cars/audi/rs6/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "11":
        msg = 'https://auto.ru/cars/audi/rs7/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "12":
        msg = 'https://auto.ru/cars/bentley/bentayga/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "13":
        msg = 'https://auto.ru/cars/bentley/bentayga/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "14":
        msg = 'https://auto.ru/cars/bentley/continental/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "15":
        msg = 'https://auto.ru/cars/bentley/continental_gt/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "16":
        msg = 'https://auto.ru/cars/bentley/continental_flying_spur/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "17":
        msg = 'https://auto.ru/cars/bentley/mulsanne/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "18":
        msg = 'https://auto.ru/cars/bmw/1er/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "19":
        msg = 'https://auto.ru/cars/bmw/2er/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "20":
        msg = 'https://auto.ru/cars/bmw/3er/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "21":
        msg = 'https://auto.ru/cars/bmw/4/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "22":
        msg = 'https://auto.ru/cars/bmw/5er/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "23":
        msg = 'https://auto.ru/cars/bmw/6er/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "24":
        msg = 'https://auto.ru/cars/bmw/7er/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "25":
        msg = 'https://auto.ru/cars/bmw/x1/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "26":
        msg = 'https://auto.ru/cars/bmw/x2/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "27":
        msg = 'https://auto.ru/cars/bmw/x3/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "28":
        msg = 'https://auto.ru/cars/bmw/x4/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "29":
        msg = 'https://auto.ru/cars/bmw/x5/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "30":
        msg = 'https://auto.ru/cars/bmw/x6/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "31":
        msg = 'https://auto.ru/cars/bmw/x7/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "32":
        msg = 'https://auto.ru/cars/bmw/z3/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "33":
        msg = 'https://auto.ru/cars/bmw/z4/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "34":
        msg = 'https://auto.ru/cars/bmw/m2/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "35":
        msg = 'https://auto.ru/cars/bmw/m3/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "36":
        msg = 'https://auto.ru/cars/bmw/m4/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "37":
        msg = 'https://auto.ru/cars/bmw/m5/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "38":
        msg = 'https://auto.ru/cars/bmw/m6/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "39":
        msg = 'https://auto.ru/cars/bmw/m8/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "40":
        msg = 'https://auto.ru/cars/bmw/x3_m/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "41":
        msg = 'https://auto.ru/cars/bmw/x5_m/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "42":
        msg = 'https://auto.ru/cars/bmw/x6_m/all/'
        bot.send_message(call.from_user.id, msg)



    if call.data == "43":
        msg = 'https://auto.ru/cars/cadillac/escalade/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "44":
        msg = 'https://auto.ru/cars/cadillac/srx/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "45":
        msg = 'https://auto.ru/cars/cadillac/sts/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "46":
        msg = 'https://auto.ru/cars/cadillac/xt5/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "47":
        msg = 'https://auto.ru/cars/cadillac/xt6/all/'
        bot.send_message(call.from_user.id, msg)



    if call.data == "48":
        msg = 'https://auto.ru/cars/ford/focus/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "49":
        msg = 'https://auto.ru/cars/ford/fusion/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "50":
        msg = 'https://auto.ru/cars/ford/mustang/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "51":
        msg = 'https://auto.ru/cars/ford/galaxy/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "52":
        msg = 'https://auto.ru/cars/ford/kuga/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "53":
        msg = 'https://auto.ru/cars/ford/s_max/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "54":
        msg = 'https://auto.ru/cars/honda/accord/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "55":
        msg = 'https://auto.ru/cars/honda/civic/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "56":
        msg = 'https://auto.ru/cars/honda/cr_v/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "57":
        msg = 'https://auto.ru/cars/honda/fit/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "58":
        msg = 'https://auto.ru/cars/honda/pilot/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "59":
        msg = 'https://auto.ru/cars/honda/shuffle/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "60":
        msg = 'https://auto.ru/cars/hyundai/accent/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "61":
        msg = 'https://auto.ru/cars/hyundai/elantra/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "62":
        msg = 'https://auto.ru/cars/hyundai/ix35/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "63":
        msg = 'https://auto.ru/cars/hyundai/santa_fe/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "64":
        msg = 'https://auto.ru/cars/hyundai/solaris/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "65":
        msg = 'https://auto.ru/cars/hyundai/sonata/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "66":
        msg = 'https://auto.ru/cars/hyundai/tucson/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "67":
        msg = 'https://auto.ru/cars/land_rover/defender/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "68":
        msg = 'https://auto.ru/cars/land_rover/discovery/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "69":
        msg = 'https://auto.ru/cars/land_rover/discovery_sport/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "70":
        msg = 'https://auto.ru/cars/land_rover/range_rover/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "71":
        msg = 'https://auto.ru/cars/land_rover/evoque/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "72":
        msg = 'https://auto.ru/cars/land_rover/range_rover_velar/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "73":
        msg = 'https://auto.ru/cars/land_rover/range_rover_sport/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "74":
        msg = 'https://auto.ru/cars/mercedes/a_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "75":
        msg = 'https://auto.ru/cars/mercedes/b_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "76":
        msg = 'https://auto.ru/cars/mercedes/c_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "77":
        msg = 'https://auto.ru/cars/mercedes/e_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "78":
        msg = 'https://auto.ru/cars/mercedes/s_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "79":
        msg = 'https://auto.ru/cars/mercedes/v_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "80":
        msg = 'https://auto.ru/cars/mercedes/cla_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "81":
        msg = 'https://auto.ru/cars/mercedes/cls_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "82":
        msg = 'https://auto.ru/cars/mercedes/gla_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "83":
        msg = 'https://auto.ru/cars/mercedes/gle_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "84":
        msg = 'https://auto.ru/cars/mercedes/gls_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "85":
        msg = 'https://auto.ru/cars/mercedes/g_klasse/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "86":
        msg = 'https://auto.ru/cars/mercedes/c_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "87":
        msg = 'https://auto.ru/cars/mercedes/e_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "88":
        msg = 'https://auto.ru/cars/mercedes/s_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "89":
        msg = 'https://auto.ru/cars/mercedes/cla_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "90":
        msg = 'https://auto.ru/cars/mercedes/cls_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "91":
        msg = 'https://auto.ru/cars/mercedes/gla_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "92":
        msg = 'https://auto.ru/cars/mercedes/gle_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "93":
        msg = 'https://auto.ru/cars/mercedes/gls_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "94":
        msg = 'https://auto.ru/cars/mercedes/g_klasse_amg/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "95":
        msg = 'https://auto.ru/cars/mercedes/amg_gt/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "96":
        msg = 'https://auto.ru/cars/porsche/911/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "97":
        msg = 'https://auto.ru/cars/porsche/911_gt2/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "98":
        msg = 'https://auto.ru/cars/porsche/911_gt3/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "99":
        msg = 'https://auto.ru/cars/porsche/cayenne/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "100":
        msg = 'https://auto.ru/cars/porsche/cayman/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "101":
        msg = 'https://auto.ru/cars/porsche/panamera/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "102":
        msg = 'https://auto.ru/cars/porsche/taycan/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "103":
        msg = 'https://auto.ru/cars/toyota/camry/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "104":
        msg = 'https://auto.ru/cars/toyota/corolla/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "105":
        msg = 'https://auto.ru/cars/toyota/land_cruiser/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "106":
        msg = 'https://auto.ru/cars/toyota/land_cruiser_prado/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "107":
        msg = 'https://auto.ru/cars/toyota/prius/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "108":
        msg = 'https://auto.ru/cars/toyota/rav_4/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "109":
        msg = 'https://auto.ru/cars/ferrari/360_modena/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "110":
        msg = 'https://auto.ru/cars/ferrari/599/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "111":
        msg = 'https://auto.ru/cars/ferrari/812_superfast/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "112":
        msg = 'https://auto.ru/cars/ferrari/california/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "113":
        msg = 'https://auto.ru/cars/ferrari/f8_tributo/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "114":
        msg = 'https://auto.ru/cars/ferrari/ff/all/'
        bot.send_message(call.from_user.id, msg)


    if call.data == "115":
        msg = 'https://auto.ru/cars/rolls_royce/cullinan/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "116":
        msg = 'https://auto.ru/cars/rolls_royce/ghost/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "117":
        msg = 'https://auto.ru/cars/rolls_royce/phantom/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "118":
        msg = 'https://auto.ru/cars/rolls_royce/wraith/all/'
        bot.send_message(call.from_user.id, msg)
    if call.data == "119":
        msg = 'https://auto.ru/cars/rolls_royce/dawn/all/'
        bot.send_message(call.from_user.id, msg)



    if call.data == 'audi':
        keyboard = types.InlineKeyboardMarkup()
        key_audi = types.InlineKeyboardButton(text='A3 💥', callback_data='1')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='A4 💥', callback_data='2')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='A5 💥', callback_data='3')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='A6 💥', callback_data='4')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='A7 💥', callback_data='5')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='A8 💥', callback_data='6')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='Q3 💥', callback_data='7')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='Q5 💥', callback_data='8')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='Q7 💥', callback_data='9')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='RS5 💥', callback_data='10')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='RS6 💥', callback_data='11')
        keyboard.add(key_audi)
        key_audi = types.InlineKeyboardButton(text='RS7 💥', callback_data='12')
        keyboard.add(key_audi)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'bentley':
        keyboard = types.InlineKeyboardMarkup()
        key_bentley = types.InlineKeyboardButton(text='Bentayga 🔥', callback_data='13')
        keyboard.add(key_bentley)
        key_bentley = types.InlineKeyboardButton(text='Continental 🔥', callback_data='14')
        keyboard.add(key_bentley)
        key_bentley = types.InlineKeyboardButton(text='Continental GT 🔥', callback_data='15')
        keyboard.add(key_bentley)
        key_bentley = types.InlineKeyboardButton(text='Continental Flying Spur 🔥', callback_data='16')
        keyboard.add(key_bentley)
        key_bentley = types.InlineKeyboardButton(text='Mulsanne 🔥', callback_data='17')
        keyboard.add(key_bentley)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'bmw':
        keyboard = types.InlineKeyboardMarkup()
        key_bmw = types.InlineKeyboardButton(text='1 series ⚡', callback_data= '18')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='2 series ⚡', callback_data='19')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='3 series ⚡', callback_data='20')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='4 series ⚡', callback_data='21')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='5 series ⚡', callback_data='22')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='6 series ⚡', callback_data='23')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='7 series ⚡', callback_data='24')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X1 ⚡', callback_data='25')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X2 ⚡', callback_data='26')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X3 ⚡', callback_data='27')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X4 ⚡', callback_data='28')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X5 ⚡', callback_data='29')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X6 ⚡', callback_data='30')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X7 ⚡', callback_data='31')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='Z3 ⚡', callback_data='32')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='Z4 ⚡', callback_data='33')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='M2 ⚡', callback_data='34')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='M3 ⚡', callback_data='35')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='M4 ⚡', callback_data='36')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='M5 ⚡', callback_data='37')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='M6 ⚡', callback_data='38')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='M8 ⚡', callback_data='39')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X3M ⚡', callback_data='40')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X5M ⚡', callback_data='41')
        keyboard.add(key_bmw)
        key_bmw = types.InlineKeyboardButton(text='X6M ⚡', callback_data='42')
        keyboard.add(key_bmw)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'cadillac':
        keyboard = types.InlineKeyboardMarkup()
        key_cadillac = types.InlineKeyboardButton(text='Escalade 🌪', callback_data='43')
        keyboard.add(key_cadillac)
        key_cadillac = types.InlineKeyboardButton(text='SRX 🌪', callback_data='44')
        keyboard.add(key_cadillac)
        key_cadillac = types.InlineKeyboardButton(text='STS 🌪', callback_data='45')
        keyboard.add(key_cadillac)
        key_cadillac = types.InlineKeyboardButton(text='XT5 🌪', callback_data='46')
        keyboard.add(key_cadillac)
        key_cadillac = types.InlineKeyboardButton(text='XT6 🌪', callback_data='47')
        keyboard.add(key_cadillac)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'ford':
        keyboard = types.InlineKeyboardMarkup()
        key_ford = types.InlineKeyboardButton(text='Focus 🪵', callback_data='48')
        keyboard.add(key_ford)
        key_ford = types.InlineKeyboardButton(text='Fusion 🪵', callback_data='49')
        keyboard.add(key_ford)
        key_ford = types.InlineKeyboardButton(text='Mustang 🪵', callback_data='50')
        keyboard.add(key_ford)
        key_ford = types.InlineKeyboardButton(text='Galaxy 🪵', callback_data='51')
        keyboard.add(key_ford)
        key_ford = types.InlineKeyboardButton(text='Kuga 🪵', callback_data='52')
        keyboard.add(key_ford)
        key_ford = types.InlineKeyboardButton(text='S-Max 🪵', callback_data='53')
        keyboard.add(key_ford)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'honda':
        keyboard = types.InlineKeyboardMarkup()
        key_honda = types.InlineKeyboardButton(text='Accord 🐉', callback_data='54')
        keyboard.add(key_honda)
        key_honda = types.InlineKeyboardButton(text='Civic 🐉', callback_data='55')
        keyboard.add(key_honda)
        key_honda = types.InlineKeyboardButton(text='CR-V 🐉', callback_data='56')
        keyboard.add(key_honda)
        key_honda = types.InlineKeyboardButton(text='Fit 🐉', callback_data='57')
        keyboard.add(key_honda)
        key_honda = types.InlineKeyboardButton(text='Pilot 🐉', callback_data='58')
        keyboard.add(key_honda)
        key_honda = types.InlineKeyboardButton(text='Shuttle 🐉', callback_data='59')
        keyboard.add(key_honda)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'hyundai':
        keyboard = types.InlineKeyboardMarkup()
        key_hyundai = types.InlineKeyboardButton(text='Accent 🫀', callback_data='60')
        keyboard.add(key_hyundai)
        key_hyundai = types.InlineKeyboardButton(text='Elantra 🫀', callback_data='61')
        keyboard.add(key_hyundai)
        key_hyundai = types.InlineKeyboardButton(text='Ix-35 🫀', callback_data='62')
        keyboard.add(key_hyundai)
        key_hyundai = types.InlineKeyboardButton(text='Santa-fe 🫀', callback_data='63')
        keyboard.add(key_hyundai)
        key_hyundai = types.InlineKeyboardButton(text='Solaris 🫀', callback_data='64')
        keyboard.add(key_hyundai)
        key_hyundai = types.InlineKeyboardButton(text='Sonata 🫀', callback_data='65')
        keyboard.add(key_hyundai)
        key_hyundai = types.InlineKeyboardButton(text='Tucson 🫀', callback_data='66')
        keyboard.add(key_hyundai)
        bot.send_message(call.from_user.id, text='Выбери модель!!', reply_markup=keyboard)

    if call.data == 'landrover':
        keyboard = types.InlineKeyboardMarkup()
        key_landrover = types.InlineKeyboardButton(text='Defender 🤘', callback_data='67')
        keyboard.add(key_landrover)
        key_landrover = types.InlineKeyboardButton(text='Discovery 🤘', callback_data='68')
        keyboard.add(key_landrover)
        key_landrover = types.InlineKeyboardButton(text='Discovery-sport 🤘', callback_data='69')
        keyboard.add(key_landrover)
        key_landrover = types.InlineKeyboardButton(text='Range-Rover 🤘', callback_data='70')
        keyboard.add(key_landrover)
        key_landrover = types.InlineKeyboardButton(text='Range-Rover Evoque 🤘', callback_data='71')
        keyboard.add(key_landrover)
        key_landrover = types.InlineKeyboardButton(text='Range-Rover Velar 🤘', callback_data='72')
        keyboard.add(key_landrover)
        key_landrover = types.InlineKeyboardButton(text='Range-Rover sport 🤘', callback_data='73')
        keyboard.add(key_landrover)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'mercedesbenz':
        keyboard = types.InlineKeyboardMarkup()
        key_mercedesbenz = types.InlineKeyboardButton(text='A class 🦈', callback_data= '74')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='B class 🦈', callback_data='75')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='C class 🦈', callback_data='76')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='E class 🦈', callback_data='77')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='S class AMG 🦈', callback_data='78')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='V class 🦈', callback_data='79')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='Cla class 🦈', callback_data='80')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='Cls class 🦈', callback_data='81')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='GLA class 🦈', callback_data='82')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='GLE class 🦈', callback_data='83')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='GLS class 🦈', callback_data='84')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='G class 🦈', callback_data='85')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='C class AMG 🦈', callback_data='86')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='E class AMG 🦈', callback_data='87')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='S class AMG 🦈', callback_data='88')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='Cla class AMG 🦈', callback_data='89')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='Cls class AMG 🦈', callback_data='90')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='GLA class AMG 🦈', callback_data='91')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='GLE class AMG 🦈', callback_data='92')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='GLS class AMG 🦈', callback_data='93')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='G class AMG 🦈', callback_data='94')
        keyboard.add(key_mercedesbenz)
        key_mercedesbenz = types.InlineKeyboardButton(text='AMG GT63 S 🦈', callback_data='95')
        keyboard.add(key_mercedesbenz)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'porsche':
        keyboard = types.InlineKeyboardMarkup()
        key_porsche = types.InlineKeyboardButton(text='911 ⚰️', callback_data='96')
        keyboard.add(key_porsche)
        key_porsche = types.InlineKeyboardButton(text='911 GT2 ⚰', callback_data='97')
        keyboard.add(key_porsche)
        key_porsche = types.InlineKeyboardButton(text='911 GT3 ⚰', callback_data='98')
        keyboard.add(key_porsche)
        key_porsche = types.InlineKeyboardButton(text='Cayenne ⚰', callback_data='99')
        keyboard.add(key_porsche)
        key_porsche = types.InlineKeyboardButton(text='Cayman ⚰', callback_data='100')
        keyboard.add(key_porsche)
        key_porsche = types.InlineKeyboardButton(text='Panamera ⚰', callback_data='101')
        keyboard.add(key_porsche)
        key_porsche = types.InlineKeyboardButton(text='Taycan ⚰', callback_data='102')
        keyboard.add(key_porsche)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'toyota':
        keyboard = types.InlineKeyboardMarkup()
        key_toyota = types.InlineKeyboardButton(text='Camry 🧨', callback_data='103')
        keyboard.add(key_toyota)
        key_toyota = types.InlineKeyboardButton(text='Corolla 🧨', callback_data='104')
        keyboard.add(key_toyota)
        key_toyota = types.InlineKeyboardButton(text='Land Cruiser 🧨', callback_data='105')
        keyboard.add(key_toyota)
        key_toyota = types.InlineKeyboardButton(text='Land Cruiser Prado 🧨', callback_data='106')
        keyboard.add(key_toyota)
        key_toyota = types.InlineKeyboardButton(text='Prius 🧨', callback_data='107')
        keyboard.add(key_toyota)
        key_toyota = types.InlineKeyboardButton(text='RAV 4 🧨', callback_data='108')
        keyboard.add(key_toyota)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'ferrari':
        keyboard = types.InlineKeyboardMarkup()
        key_ferrari = types.InlineKeyboardButton(text='360 💸', callback_data='109')
        keyboard.add(key_ferrari)
        key_ferrari = types.InlineKeyboardButton(text='599 💸', callback_data='110')
        keyboard.add(key_ferrari)
        key_ferrari = types.InlineKeyboardButton(text='812 💸', callback_data='111')
        keyboard.add(key_ferrari)
        key_ferrari = types.InlineKeyboardButton(text='California 💸', callback_data='112')
        keyboard.add(key_ferrari)
        key_ferrari = types.InlineKeyboardButton(text='F8 💸', callback_data='113')
        keyboard.add(key_ferrari)
        key_ferrari = types.InlineKeyboardButton(text='FF 💸', callback_data='114')
        keyboard.add(key_ferrari)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

    if call.data == 'rr':
        keyboard = types.InlineKeyboardMarkup()
        key_rollsroyce = types.InlineKeyboardButton(text='Cullinan 💰', callback_data='115')
        keyboard.add(key_rollsroyce)
        key_rollsroyce = types.InlineKeyboardButton(text='Ghost 💰', callback_data='116')
        keyboard.add(key_rollsroyce)
        key_rollsroyce = types.InlineKeyboardButton(text='Phantom 💰', callback_data='117')
        keyboard.add(key_rollsroyce)
        key_rollsroyce = types.InlineKeyboardButton(text='Wraith 💰', callback_data='118')
        keyboard.add(key_rollsroyce)
        key_rollsroyce = types.InlineKeyboardButton(text='Dawn 💰', callback_data='119')
        keyboard.add(key_rollsroyce)
        bot.send_message(call.from_user.id, text='Выбери модель!', reply_markup=keyboard)

bot.infinity_polling()



