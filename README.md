const {Client, Attachment} = require("discord.js");
const client = new Client();
var prefix = "!";


client.on('ready', () =>      { 
console.log(`Logged in as ${client.user.tag}!`);
});



client.on("message", msg => {
const achn = ['833783322752581695','834207093296332851'];
if (!achn.includes(msg.channel.id)) return; 
if (msg.author.bot) return;
if (msg.content.startsWith("")) {
const pic = new Attachment('https://cdn.discordapp.com/attachments/834225436983951450/834374930983813130/test.gif');
msg.channel.send(pic);
};     
});



client.login("ODMzNzU5MDY1NTgyNzMxMzA0.YH3Aow.JKBPRDWTfsqL4WQ2OOTW9CLP52c");
