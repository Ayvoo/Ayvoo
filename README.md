import telepot

bot = telebot.Telebot(6211755623:AAGYeIJcoyMhak2I9BjDINsqjEJs_V5EXvU)


define a function that will be called when a message is received
@bot.message_handler(commands=['start','help','info','status'])
def handle_command(message):
if messange.text == '/start':
bot.send_message(message.chat.id, "مرحبا انا بوت ايةاهلا بك")
elif message.text == '/help':
bot.send_message(message.chat.id, "مالذي تبحث عنه هاا؟؟؟")
elif message.text == '/info':
bot.send_message(message.chat.id, "انا بوت تيلقرام بسيط احب ذا نيبرهود هل يمكنني مساعدتك بشيء؟")
elif message.text == '/status':
bot.send_message(message.chat.id, "انا هنا بأي وقت و مستعده لتقديم المساعدة اليك")

#start the bot
bot.polling()
