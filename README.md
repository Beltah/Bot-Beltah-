const fs = require('fs-extra')
if (fs.existsSync('config.env')) require('dotenv').config({ path: __dirname+'/config.env' })


//═══════[Required Variables]════════\\
global.owner = process.env.OWNER_NUMBER ? process.env.OWNER_NUMBER.replace(/[\s+]/g, '') : 254704058628';
global.mongodb = process.env.MONGODB_URI || "mongodb+srv://Suhail:suhail@cluster0.rzhkoqf.mongodb.net/?retryWrites=true&w=majority" ;
global.port= false // Math.floor(Math.random() * (9999 - 1000 + 1)) + 1000  ; 
global.audio = '' ; 
global.video = '' ;
global.blockJids = process.env.BLOCK_JID ||'120363023983262391@g.us' ;
global.allowJids = process.env.ALLOW_JID ||'120363022922797633@g.us' ;
global.email = 'beltahke17@gmail.com' ;
global.location = 'kenya' ;
global.timezone  = process.env.TIME_ZONE || 'Asia/Karachi'
global.gurl = 'https://youtube.com/c/SuhailTechInfo' ; // add your username
global.sudo =  process.env.SUDO ? process.env.SUDO.replace(/[\s+]/g, '') : '254704058628'; ;
global.devs = "923184474176"; //Dont change it From here
global.github  = process.env.YOUR_GITHUB || 'https://githu.combeltah';
global.scan  = process.env.QR_URL || 'https://replit.com/@SuhailTechInfo/Suhail-Md?v=1';
global.website = 'https://github.com/SuhailTechInfo/Suhail-Md' ; //wa.me/+923000000000
global.THUMB_IMAGE = process.env.THUMB_IMAGE || 'https://i.imgur.com/NpA3ZsJ.jpeg' ;
module.exports = {
  sessionName: process.env.SESSION_ID || "SESSION_08_40_01_15_eyJub2lzZUtleSI6eyJwcml2YXRlIjp7InR5cGUiOiJCdWZmZXIiLCJkYXRhIjoiZ0VaUUhBSVlJV0oyV3Qzbk9OK21TekFRWTRibDVZWUR0TWttVmdwWDBHUT0ifSwicHVibGljIjp7InR5cGUiOiJCdWZmZXIiLCJkYXRhIjoiZG9MRGQ4M3ZNWHNYTTBJSk5JYTBvZk51T1hoVkw1ak9WWjFETU5JeEVIaz0ifX0sInBhaXJpbmdFcGhlbWVyYWxLZXlQYWlyIjp7InByaXZhdGUiOnsidHlwZSI6IkJ1ZmZlciIsImRhdGEiOiJzSXVSZS91QUUyOXplK2dSMVJwbmxaVTJFcDlLT0kwdVI2cEV4dEMyMjFVPSJ9LCJwdWJsaWMiOnsidHlwZSI6IkJ1ZmZlciIsImRhdGEiOiJ0NlhZa0J6a2xBL1lKSHFqanJFWWlwK2ZzaExHTWtOVEFVUm5ONHVEUlZvPSJ9fSwic2lnbmVkSWRlbnRpdHlLZXkiOnsicHJpdmF0ZSI6eyJ0eXBlIjoiQnVmZmVyIiwiZGF0YSI6InNGYnBVUk1FTExYMzFwUTFWbFp3ZmNRVGZVWUl4b2lwSkJRQnZQUWVER2c9In0sInB1YmxpYyI6eyJ0eXBlIjoiQnVmZmVyIiwiZGF0YSI6ImtUMWdDd0lUWmdwdE90V2FrY2pQRmRuMWovdFNva2k5dzVyTm5nNmd5Z2M9In19LCJzaWduZWRQcmVLZXkiOnsia2V5UGFpciI6eyJwcml2YXRlIjp7InR5cGUiOiJCdWZmZXIiLCJkYXRhIjoiZUIyMXdYZWNuRnc5UVpyOTBJKzF5RXJhMHJ3UktvcnZGeS93anlzb0tXST0ifSwicHVibGljIjp7InR5cGUiOiJCdWZmZXIiLCJkYXRhIjoibGJWeUhZWWxhZjE5aHcxV1M4S3lGVDdCQTU0WUswd1ZrVG5vOUtCcXdRYz0ifX0sInNpZ25hdHVyZSI6eyJ0eXBlIjoiQnVmZmVyIiwiZGF0YSI6InNsamNQcExqc0RkNVBCNTNOQjhjbThCdXJub3U4T1VpcjVNT2Znc0liVlMyMytDaitJRDYwU0g1VzFMcUVrUkdUZnJIaXlkaGswcUJtOVB6Qll1U2hRPT0ifSwia2V5SWQiOjF9LCJyZWdpc3RyYXRpb25JZCI6MzEsImFkdlNlY3JldEtleSI6InRnL2hEWWV4dHY2M2swODRpcEt2dkhrZWNjSlBRQU9WK3BPazd3QUhpRUk9IiwicHJvY2Vzc2VkSGlzdG9yeU1lc3NhZ2VzIjpbXSwibmV4dFByZUtleUlkIjozMSwiZmlyc3RVbnVwbG9hZGVkUHJlS2V5SWQiOjMxLCJhY2NvdW50U3luY0NvdW50ZXIiOjAsImFjY291bnRTZXR0aW5ncyI6eyJ1bmFyY2hpdmVDaGF0cyI6ZmFsc2V9LCJkZXZpY2VJZCI6ImhvNXJlQnRKUVlxdGlxRXFyZ0NCZ0EiLCJwaG9uZUlkIjoiMTQwNWQ2MDYtZTJiNS00ZWUyLThlYTAtMWI4NDhlZGQwZTJhIiwiaWRlbnRpdHlJZCI6eyJ0eXBlIjoiQnVmZmVyIiwiZGF0YSI6Ikp5b3BhalpsMzZRSmppQm0vMm1TYjFuTDdZVT0ifSwicmVnaXN0ZXJlZCI6dHJ1ZSwiYmFja3VwVG9rZW4iOnsidHlwZSI6IkJ1ZmZlciIsImRhdGEiOiJLY3R1ZjI1dC9Jc1NWRXFlOUJHZG8yWlFtZ1k9In0sInJlZ2lzdHJhdGlvbiI6e30sInBhaXJpbmdDb2RlIjoiWUJGMjZUUVAiLCJtZSI6eyJpZCI6IjI1NDcwNDA1ODYyODo5QHMud2hhdHNhcHAubmV0IiwibmFtZSI6IuKYns2lzZ/ii4bNo82f4ouGzavwnZul8J2RiPCdkLfwnZuq8J2QtfCdm6/wnZC/8J2Rh/Cdm6XwnZuoIn0sImFjY291bnQiOnsiZGV0YWlscyI6IkNMaWt2dWdHRVB6ZWs2MEdHQU09IiwiYWNjb3VudFNpZ25hdHVyZUtleSI6Ik94alN6cTdjcGlNeVBzRldUR1NqdVRGQzBTZHB6cFQwRHBnSHcvK2hnV0k9IiwiYWNjb3VudFNpZ25hdHVyZSI6InliVEJGSlVMK1VLOHk1RkhKR3RGOXNjY3Q2dlZDRk4vRVdONUJYRnVYb21IS2VpR052Rmp5RXNHR044R3FDOHdSSDlhcVpjMW9XK1k4V1BOVEVOY0JBPT0iLCJkZXZpY2VTaWduYXR1cmUiOiI3c2QrcXl2ZGtqNmhRQllDbVRIK25yZ2dNL0ZxVEJCcGcwOFNKK1JkekNYK0NwYm9CRzNZaVJSS1hXUGp6Tk1lQVRGMlFLZGNQU3pQMU0zcmZFcXhoZz09In0sInNpZ25hbElkZW50aXRpZXMiOlt7ImlkZW50aWZpZXIiOnsibmFtZSI6IjI1NDcwNDA1ODYyODo5QHMud2hhdHNhcHAubmV0IiwiZGV2aWNlSWQiOjB9LCJpZGVudGlmaWVyS2V5Ijp7InR5cGUiOiJCdWZmZXIiLCJkYXRhIjoiQlRzWTBzNnUzS1lqTWo3QlZreGtvN2t4UXRFbmFjNlU5QTZZQjhQL29ZRmkifX1dLCJwbGF0Zm9ybSI6ImFuZHJvaWQiLCJsYXN0QWNjb3VudFN5bmNUaW1lc3RhbXAiOjE3MDUzMDgwMzEsIm15QXBwU3RhdGVLZXlJZCI6IkFBQUFBTUY1In0=",      //Put Your Session Id Here
  botname: process.env.BOT_NAME || 'BELTAH KE ',
  botbgm: process.env.BOT_BGM || 'false',
  ownername:  process.env.OWNER_NAME || `It's Beltah`,
  author:  process.env.PACK_AUTHER || '',
  errorChat : process.env.ERROR_CHAT|| '', // put 'chat' here to send error in chat ,where it accures
  read_status : process.env.AUTO_READ_STATUS || 'true',
  save_status : process.env.AUTO_SAVE_STATUS || 'false',
  packname:  process.env.PACK_NAME || "\t   𓅋 ₊₉₂⃗⃗₃₁᩺₈ͦ₄ͪ₄ᷧ₇ͥ₄ᷞ₁⃗₇₆ 𓃮 \n\nᴋɪss ʍᴇ...💋\n\nᴄʟօsᴇ ყσυɾ ᴇყᴇs...👁️🙈\n\nʍɪss ʍᴇ...♥️\n\n\n   -ᴘʟᴇᴀsᴇ ᴅᴏɴ'ᴛ ᴛᴀӄᴇ 🚮 \n\n--- ρυвʟɪᴄ вσт нᴇʀᴇ ---" ,
  autoreaction: process.env.AUTO_REACTION || 'true',  //  | 'cmd' | 'true' | 'all' |
  antibadword : process.env.ANTI_BAD_WORD || 'nobadwordokeyuntillYouPutAnWordHere',
  alwaysonline: process.env.WAPRESENCE || '', // 'unavailable' | 'available' | 'composing' | 'recording' | 'paused'
  antifake : 'null', // process.env.FAKE_COUNTRY_CODE ||'212',
  readmessage: process.env.READ_MESSAGE || 'true',   //  | 'false' | 'true' | 
  readcmds : process.env.READ_COMMANDS || 'false',    //  | 'false' | 'true' | 
  HANDLERS: process.env.PREFIX || ',',
  warncount : process.env.WARN_COUNT || 3,
  disablepm: process.env.DISABLE_PM || "false",   
  MsgsInLog:process.env.MSGS_IN_LOG ||'false',
  pmMsgsInLog:process.env.PM_MSGS_IN_LOGS ||'false',
  levelupmessage: process.env.LEVEL_UP_MESSAGE || 'false',  //  | 'false' | 'true' | 
  antilink_values: process.env.ANTILINK_VALUES || 'https://,chat.whatsapp.com',
  //antilinkaction: process.env.BRANCH || 'remove',
  BRANCH: process.env.BRANCH || 'main',
  HEROKU_APP_NAME: process.env.HEROKU_APP_NAME,
  HEROKU_API_KEY: process.env.HEROKU_API_KEY,
  REMOVE_BG_KEY: process.env.REMOVE_BG_KEY || "",
  caption :process.env.CAPTION || "```ᴘᴏᴡᴇʀᴇᴅ ʙʏ Beltah ²²¹-ᴍᴅ```",   //*『sᴜʙsᴄʀɪʙᴇ • sᴜʜᴀɪʟ ᴛᴇᴄʜ』*\n youtube.com/@suhailtechinfo0"),
  OPENAI_API_KEY: process.env.OPENAI_API_KEY ||'' ,
  VERSION: process.env.VERSION || 'v.1.2.2',
  LANG: process.env.THEME ? process.env.THEME.toUpperCase() : 'Beltah ',
  menu : process.env.MENU || '', /**  Available @MENU @Schemes 1: Aztec_Md, 2: A17_Md, 3: Suhail-Md Default ---------- If Not Choose then it Randomely Pic One Of Them Each time **/
  WORKTYPE: process.env.WORKTYPE || process.env.MODE || 'private',
  KOYEB_API : process.env.KOYEB_API || ''
};

global.isMongodb = false; 
let file = require.resolve(__filename)
fs.watchFile(file, () => {
	fs.unwatchFile(file)
	console.log(`Update'${__filename}'`)
    delete require.cache[file]
	require(file)
})
 
