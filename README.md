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
end

$ex = explode("\n",file_get_contents("ملف تخزين الاعضاء.txt"));
$admin = youid;
if($text == "/start" and !in_array($ex,$from_id)){
bot('sendmessage',[
'chat_id' => $admin,
'text' => "
اهلا عزيزي المطور هناك من قام بالدخول للبوت 
- اسمه : - $name
- معرفه : - @$user
- ايديه : - $from_id
",
]);}
end 

$getch = file_get_contents("https://domain.com/api.php?from_id=".$chat_id);
/*بدل كلمة domain.com بالدومين خاصك*/
if($text == "/start" && $getch->join == "True"){
}
if($text == "/start" && $getch->join == "False"){
bot('sendMessage',[
'chat_id'=>$chat_id,
'text'=>$getch->subscribe,
]);return false;
}
end

if($text == "الغاء تثبيت الكل" ){
bot('unpinAllChatMessages',[
'chat_id'=>$chat_id,
]);
bot('sendmessage',[
'chat_id' => $chat_id,
'text' => " - تم الغاء قائمة التثبيت بنجاح",
'reply_to_message_id'=>$message->message_id,
]);}
end

$taz = array ("476328331","0000");
$first_name = $message->from->first_name;
if(in_array($from_id,$taz)){
$info = "مطور السورس";
}
elseif(in_array($from_id,$developer) ){
$info = "مطور البوت";
}
elseif(in_array($from_id,$Dev) ){
$info = "مطور الاساسي";
}
elseif(in_array($from_id,$nazar) ){
$info = "منشئ اساسي";
}
elseif(in_array($from_id,$carlos) ){
$info = "منشئ";
}
elseif($status == "creator"){
$info = "المالك";
}
elseif($status == "administrator"){
$info = "المشرف";
}
elseif(in_array($from_id,$manger) ){
$info = "المدير";
}
elseif(in_array($from_id,$admin_user) ){
$info = "ادمن";
}
elseif(in_array($from_id,$mmyaz) ){
$info = "عضو مميز";
}elseif($status == "member" ){
$info = "عضو فقط";
}
if($text=="رتبتي" ){
bot('sendmessage',[
'chat_id'=>$chat_id, 
'text'=>"
🎫┊اسمـڪ » $first_name
🎟┊رتبـتڪ » $info
➖
",
'parse_mode'=>"html",
'reply_to_message_id'=>$message->message_id,
]);
}

if($text == "مطور السورس"){
bot('sendmessage',[
'chat_id' => $chat_id,
'text' => "
- [مطور السورس معتز الدرسي ](tg://user?id=$taz[0])
",
'reply_to_message_id'=>$message->message_id,
'disable_web_page_preview'=> true ,
 'parse_mode'=>"Markdown",
]);}
end

$taz = "00000"; //you id
if($message->reply_to_message->document and $text == 'رفع الملف' and $from_id == $taz){
     $file = "https://api.telegram.org/file/bot".API_KEY."/".bot('getfile',['file_id'=>$message->reply_to_message->document->file_id])->result->file_path;
     file_put_contents($message->reply_to_message->document->file_name,file_get_contents($file));
     bot('sendMessage',[
            'chat_id'=>$chat_id,
            'text'=>'تم رفع الملف ؛ '.$message->reply_to_message->document->file_name
         ]);
 }
if($text == "رفع ملف" and $from_id == $taz){
bot('sendMessage',[
'chat_id'=>$chat_id, 
'text'=>"
☑️┋ارسل الملف الان
☑️┋بعدها قم بعمل رد على الملف واكتب 
end

$motaz = $message->text;
$gnral = "GnralEs_bot";  //يوزر بوتك دون @
$lmotaz = $update->callback_query->message->message_id;
$aldrsy = $message->chat->id;
$lslhb = $update->callback_query->data;
$sand = $update->callback_query->message->chat->id;
$PIIIIli = rand(2, 21);
if($motaz == "اغنيه"){
bot('sendvoice',[
'chat_id'=>$aldrsy,
'voice'=>"https://t.me/faheg/$PIIIIli",
'caption'=>"@$gnral", 
'disable_web_page_preview'=> true ,
'parse_mode'=>"Markdown",
'reply_markup'=>json_encode([
'inline_keyboard'=>[
[[ 'text' => 'اغنيه اخرى',callback_data => 'sand' ]],
]])]);}

if($lslhb == "sand"){
bot('deleteMessage',[
'chat_id'=>$sand,
'message_id'=>$lmotaz,
 ]);
bot('sendvoice',[
'chat_id'=>$sand,
'message_id'=>$lmotaz,
'voice'=>"https://t.me/faheg/$PIIIIli",
'caption'=>"@$gnral", 
'disable_web_page_preview'=> true ,
'parse_mode'=>"Markdown",
'reply_markup'=>json_encode([
'inline_keyboard'=>[
[[ 'text' => 'اغنيه اخرى',callback_data => 'sand' ]],
]])]);}

end

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
