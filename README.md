const Diacord = require('discord.js');
const megafb = require("megadb")
let db = new megadb.crearDB("prefixes")
module.exports = {
name: "set-prefix",


async execute(clientmessage, args){
let server = message.guild.id


if(!message.member.perssions.has("ADMINISTRADOR")){
return message.channel.send("no tienes los permisos nesesarios")
let prefix = args.join(" ")


if(prefix){
return message.channel.send("escribe un prefix")
}


db.estableser('${server}',prefix)

message.channel.send("prefix cambiado a "+prefix)
