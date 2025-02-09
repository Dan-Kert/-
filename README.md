# -import telebot

# Вставь свой API-токен
TOKEN = '7593232506:AAExkR6nse66p4PGsMZFPWcOkw9DWgHFf6E'
bot = telebot.TeleBot(TOKEN)

# Обработчик команды /start
@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "Привет! Я бот, работающий на @dankert и @dan_kert ")

# Запуск бота
bot.polling()
