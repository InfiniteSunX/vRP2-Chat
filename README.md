To make that works, you only need to change in chat/sv_chat.lua this line:
TriggerClientEvent('chatMessage', -1, author,  { 255, 255, 255 }, message)
with this line:
TriggerEvent("vrp_chat:chat_message",source,author,message)
...inspired by foxoak
