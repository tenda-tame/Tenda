# Tenda
if text == 'الاوامر' and GetSourseMember(msg) then     
if not Addictive(msg) then
send(msg.chat_id_, msg.id_,'• عذرا الاوامر هذا لا المنشئين ') 
return false
end
local Text =[[
#besso
●━━━━━𝑩𝑺━━━━━●
•  ① > لعرض اوامر الحمايه
•  ② > لعرض اوامر الادمنيه
•  ③ > لعرض اوامر المدراء
•  ④ > لعرض اوامر المنشئين
•  ⑤ > لعرض اوامر المطورين
●○━━━━━𝑩𝑺━━━━━●
𝘊𝘩 - [Besso](t.me/BESSO500K) •
]]
keyboard = {} 
keyboard.inline_keyboard = {
{{text = '1', callback_data="/help1"},{text = '2', callback_data="/help2"},{text = '3', callback_data="/help3"}},
{{text = '4', callback_data="/help4"},{text = '5', callback_data="/help5"}},
{{text = 'اوامر التسليه', callback_data="/help10"}},
}
local msg_id = msg.id_/2097152/0.6
https.request("https://api.telegram.org/bot"..token..'/sendMessage?chat_id=' .. msg.chat_id_ .. '&text=' .. URL.escape(Text).."&reply_to_message_id="..msg_id.."&parse_mode=markdown&disable_web_page_preview=true&reply_markup="..JSON.encode(keyboard))
return false
end
