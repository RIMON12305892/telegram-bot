 # bot.py
 import telebot
import os

TOKEN = os.getenv("8348969341:AAF_8IMb1SEA4IppGsjKUV4LuFvZ_-IJX5I")
bot = telebot.TeleBot(8348969341:AAF_8IMb1SEA4IppGsjKUV4LuFvZ_-IJX5I)

@bot.message_handler(commands=['start'])
def start(message):
    bot.send_message(message.chat.id, "👋 Привіт! Я твій бот.")

bot.polling()
