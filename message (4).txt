

const Discord = require("discord.js");
//require('dotenv').config()
const client = new Discord.Client();
const client2 = new Discord.Client({});
const client3 = new Discord.Client();
const client4 = new Discord.Client();
const client5 = new Discord.Client();
const client6 = new Discord.Client();






const humanizeDuration = require("humanize-duration");



client.on("ready", () => {
  console.log(`Logged in as : ${client.user.username}`);
  client.user.setActivity(`بيوي و حكسر بس`);
  client.user.setStatus("idle");
});
const owners = ["455108784579149835", "527826654660132890"]
var prefix = "-"; 

client.on("message", async message => {
    if(!owners.includes(message.author.id)) return;
    if(message.channel.type == "dm") return
    if (message.content.startsWith(prefix + "settoken1")) {
        let args = message.content.slice(prefix.length).trim().split(/ +/);
        let token = args[1]
        if(!token) return
        await client2.destroy()
        await message.delete()
         await client2.login(token).then( async m => { 
             
            if(client2.user.bot !== true) {
                await message.reply("**توكن ذا مو حق بوت**") 
                return
            }
            
        
        
        }).catch(error => {
            return message.channel.send("**توكن خربان / مبند**")
           })  
           if(client2.user.bot !== true) return
        
             await message.reply(new Discord.RichEmbed().setTitle('معلومات عن توكن البوت').setDescription(`
             **Name:** ${client2.user.username}
             **ID:** ${client2.user.id} 
             **Age:** ${humanizeDuration(Date.now() - client2.user.createdTimestamp, { units: ['y', 'mo', 'd'], round: true})}
             **Invite Link:** [رابط هنا](https://discord.com/api/oauth2/authorize?client_id=${client2.user.id}&permissions=384064&scope=bot)
             
             
             `).setColor('GREEN').setThumbnail(client2.user.avatarURL).setFooter(message.guild.name, message.guild.iconURL).setAuthor(`تم تشغيل بوت 🟢`).setTimestamp())
       
         
     
     
        }
        if (message.content.startsWith(prefix + "settoken2")) {
            let args = message.content.slice(prefix.length).trim().split(/ +/);
            let token = args[1]
            if(!token) return
            await client3.destroy()
            await message.delete()
             await client3.login(token).then( async m => { 
                 
                if(client3.user.bot !== true) {
                    await message.reply("**توكن ذا مو حق بوت**") 
                    return
                }
                
            
            
            }).catch(error => {
                return message.channel.send("**توكن خربان / مبند**")
               })  
               if(client3.user.bot !== true) return
            
                 await message.reply(new Discord.RichEmbed().setTitle('معلومات عن توكن البوت').setDescription(`
                 **Name:** ${client3.user.username}
                 **ID:** ${client3.user.id} 
                 **Age:** ${humanizeDuration(Date.now() - client3.user.createdTimestamp, { units: ['y', 'mo', 'd'], round: true})}
                 **Invite Link:** [رابط هنا](https://discord.com/api/oauth2/authorize?client_id=${client3.user.id}&permissions=384064&scope=bot)
                 
                 
                 `).setColor('GREEN').setThumbnail(client3.user.avatarURL).setFooter(message.guild.name, message.guild.iconURL).setAuthor(`تم تشغيل بوت 🟢`).setTimestamp())
           
             
         
         
            }
            if (message.content.startsWith(prefix + "settoken3")) {
                
                let args = message.content.slice(prefix.length).trim().split(/ +/);
                let token = args[1]
                if(!token) return
                await client4.destroy()
                await message.delete()
                 await client4.login(token).then( async m => { 
                     
                    if(client4.user.bot !== true) {
                        await message.reply("**توكن ذا مو حق بوت**") 
                        return
                    }
                    
                
                
                }).catch(error => {
                    return message.channel.send("**توكن خربان / مبند**")
                   })  
                   if(client4.user.bot !== true) return
                
                     await message.reply(new Discord.RichEmbed().setTitle('معلومات عن توكن البوت').setDescription(`
                     **Name:** ${client4.user.username}
                     **ID:** ${client4.user.id} 
                     **Age:** ${humanizeDuration(Date.now() - client4.user.createdTimestamp, { units: ['y', 'mo', 'd'], round: true})}
                     **Invite Link:** [رابط هنا](https://discord.com/api/oauth2/authorize?client_id=${client4.user.id}&permissions=384064&scope=bot)
                     
                     
                     `).setColor('GREEN').setThumbnail(client4.user.avatarURL).setFooter(message.guild.name, message.guild.iconURL).setAuthor(`تم تشغيل بوت 🟢`).setTimestamp())
               
                 
             
             
                }
                if (message.content.startsWith(prefix + "settoken4")) {
                    let args = message.content.slice(prefix.length).trim().split(/ +/);
                    let token = args[1]
                    if(!token) return
                    await client5.destroy()
                    await message.delete()
                     await client5.login(token).then( async m => { 
                         
                        if(client5.user.bot !== true) {
                            await message.reply("**توكن ذا مو حق بوت**") 
                            return
                        }
                        
                    
                    
                    }).catch(error => {
                        return message.channel.send("**توكن خربان / مبند**")
                       })  
                       if(client5.user.bot !== true) return
                    
                         await message.reply(new Discord.RichEmbed().setTitle('معلومات عن توكن البوت').setDescription(`
                         **Name:** ${client5.user.username}
                         **ID:** ${client5.user.id} 
                         **Age:** ${humanizeDuration(Date.now() - client5.user.createdTimestamp, { units: ['y', 'mo', 'd'], round: true})}
                         **Invite Link:** [رابط هنا](https://discord.com/api/oauth2/authorize?client_id=${client5.user.id}&permissions=384064&scope=bot)
                         
                         
                         `).setColor('GREEN').setThumbnail(client5.user.avatarURL).setFooter(message.guild.name, message.guild.iconURL).setAuthor(`تم تشغيل بوت 🟢`).setTimestamp())
                   
                     
                 
                 
                    }
                    if (message.content.startsWith(prefix + "settoken5")) {
                        let args = message.content.slice(prefix.length).trim().split(/ +/);
                        let token = args[1]
                        if(!token) return
                        await client6.destroy()
                        await message.delete()
                         await client6.login(token).then( async m => { 
                             
                            if(client6.user.bot !== true) {
                                await message.reply("**توكن ذا مو حق بوت**") 
                                return
                            }
                            
                        
                        
                        }).catch(error => {
                            return message.channel.send("**توكن خربان / مبند**")
                           })  
                           if(client6.user.bot !== true) return
                        
                             await message.reply(new Discord.RichEmbed().setTitle('معلومات عن توكن البوت').setDescription(`
                             **Name:** ${client6.user.username}
                             **ID:** ${client6.user.id} 
                             **Age:** ${humanizeDuration(Date.now() - client6.user.createdTimestamp, { units: ['y', 'mo', 'd'], round: true})}
                             **Invite Link:** [رابط هنا](https://discord.com/api/oauth2/authorize?client_id=${client6.user.id}&permissions=384064&scope=bot)
                             
                             
                             `).setColor('GREEN').setThumbnail(client6.user.avatarURL).setFooter(message.guild.name, message.guild.iconURL).setAuthor(`تم تشغيل بوت 🟢`).setTimestamp())
                       
                         
                     
                     
                        }
       
   
  
                    })
                    client2.on("message", async me => {
                        if(!owners.includes(me.author.id)) return;
                        let errornumber = 1
                        

                        if (!me.guild) return;
                            let args = me.content.split(" ").slice(1).join(" ");
                            if (me.content.startsWith(prefix + "obc1")) { 
                         if(!args) return me.reply(new Discord.RichEmbed()
                        .addField(`Online Boardcat`,`${prefix}obc1 [message]`))
                        let number = 1
                        let brodeembed = new Discord.RichEmbed()
                        .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`)
                        
                        me.channel.send(brodeembed).then(async ll => { 
                            
                            
                        await  me.guild.members.filter(m => m.presence.status !== 'offline').forEach( async m => {
                          if(m.id != client.user.id && !m.user.bot)
                          
                          await m.send(`${args}\n ${m}`).then(()=>{
                             ll.edit(new Discord.RichEmbed()
                             .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
                        number++
                       
                                        }).catch(function(){
                                            errornumber++
                                            ll.edit(new Discord.RichEmbed()
                                            .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n **فشل ارسال الى \`${errornumber}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                                        })
                          })})
                                       
                        
                          
                          }
                          if (!me.guild) return;
              if (me.content.startsWith(prefix+"bc1")) {
let number1 = 0
let errornumber1 = 1

let number02 = 0
    if(!args) return me.reply(new Discord.RichEmbed()
    .addField(`Boardcat to all`,`${prefix}bc1 [message]`));
    let brodeembed = new Discord.RichEmbed()
    .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`)
    
    me.channel.send(brodeembed).then(async ll => {
        me.guild.members.forEach( m => {
   if(m.id != client.user.id && !m.user.bot)m.send(`${args}\n ${m}`).then(()=>{
    ll.edit(new Discord.RichEmbed()
    .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL))
number1++
                }).catch(function(){
                    errornumber1++
                    ll.edit(new Discord.RichEmbed()
                    .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n **فشل ارسال الى \`${errornumber1}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                });
            
     })
    })
   
    
    };    
    if (me.content.startsWith(prefix+"setname1")) {
      if(!args) return me.reply(`**${prefix}setname1 [name]**`)
    await client2.user.setUsername(args)
    me.channel.send(`تم تغير اسم الى ${args}`)
    }
    if (me.content.startsWith(prefix+"setavt1")) {
      if(!args) return me.reply(`**${prefix}setavt1 [avatar URL]**`)
      client2.user.setAvatar(args).then(
        me.channel.send(new Discord.RichEmbed().setTitle('تم تغير صورة الى').setThumbnail(args)).catch(error => {
          return me.channel.send(error)
         })  
      )
    }



                                   
                          
                          });
                          client3.on("message", async me => {
                            if(!owners.includes(me.author.id)) return;
                            let errornumber = 1
                            
    
                            if (!me.guild) return;
                                let args = me.content.split(" ").slice(1).join(" ");
                                if (me.content.startsWith(prefix + "obc2")) { 
                             if(!args) return me.reply(new Discord.RichEmbed()
                            .addField(`Online Boardcat`,`${prefix}obc1 [message]`))
                            let number = 1
                            let brodeembed = new Discord.RichEmbed()
                            .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`)
                            
                            me.channel.send(brodeembed).then(async ll => { 
                                
                                
                            await  me.guild.members.filter(m => m.presence.status !== 'offline').forEach( async m => {
                              if(m.id != client.user.id && !m.user.bot)
                              
                              await m.send(`${args}\n ${m}`).then(()=>{
                                 ll.edit(new Discord.RichEmbed()
                                 .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
                            number++
                           
                                            }).catch(function(){
                                                errornumber++
                                                ll.edit(new Discord.RichEmbed()
                                                .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n **فشل ارسال الى \`${errornumber}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                                            })
                              })})
                                           
                            
                              
                              }
                              if (!me.guild) return;
                  if (me.content.startsWith(prefix+"bc2")) {
    let number1 = 0
    let errornumber1 = 1
    
    let number02 = 0
        if(!args) return me.reply(new Discord.RichEmbed()
        .addField(`Boardcat to all`,`${prefix}bc1 [message]`));
        let brodeembed = new Discord.RichEmbed()
        .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`)
        
        me.channel.send(brodeembed).then(async ll => {
            me.guild.members.forEach( m => {
       if(m.id != client.user.id && !m.user.bot)m.send(`${args}\n ${m}`).then(()=>{
        ll.edit(new Discord.RichEmbed()
        .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
    number1++
                    }).catch(function(){
                        errornumber1++
                        ll.edit(new Discord.RichEmbed()
                        .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n **فشل ارسال الى \`${errornumber1}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                    });
                
         })
        })
       
        
        };  
        if (me.content.startsWith(prefix+"setname2")) {
          if(!args) return me.reply(`**${prefix}setname2 [name]**`)
        await client3.user.setUsername(args)
        me.channel.send(`تم تغير اسم الى ${args}`)
        }
        if (me.content.startsWith(prefix+"setavt2")) {
          if(!args) return me.reply(`**${prefix}setavt2 [avatar URL]**`)
          client3.user.setAvatar(args).then(
            me.channel.send(new Discord.RichEmbed().setTitle('تم تغير صورة الى').setThumbnail(args)).catch(error => {
              return me.channel.send(error)
             })  
          )
        }  
                
                
                                
                              });
                              client4.on("message", async me => {
                                
                                if(!owners.includes(me.author.id)) return;
                                let errornumber = 1
                                
        
                                if (!me.guild) return;
                                    let args = me.content.split(" ").slice(1).join(" ");
                                    if (me.content.startsWith(prefix + "obc3")) { 
                                 if(!args) return me.reply(new Discord.RichEmbed()
                                .addField(`Online Boardcat`,`${prefix}obc3 [message]`))
                                let number = 1
                                let brodeembed = new Discord.RichEmbed()
                                .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`)
                                
                                me.channel.send(brodeembed).then(async ll => { 
                                    
                                    
                                await  me.guild.members.filter(m => m.presence.status !== 'offline').forEach( async m => {
                                  if(m.id != client.user.id && !m.user.bot)
                                  
                                  await m.send(`${args}\n ${m}`).then(()=>{
                                     ll.edit(new Discord.RichEmbed()
                                     .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
                                number++
                               
                                                }).catch(function(){
                                                    errornumber++
                                                    ll.edit(new Discord.RichEmbed()
                                                    .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n **فشل ارسال الى \`${errornumber}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                                                })
                                  })})
                                               
                                
                                  
                                  }
                                  if (!me.guild) return;
                      if (me.content.startsWith(prefix+"bc3")) {
        let number1 = 0
        let errornumber1 = 1
        
        let number02 = 0
            if(!args) return me.reply(new Discord.RichEmbed()
            .addField(`Boardcat to all`,`${prefix}bc3 [message]`));
            let brodeembed = new Discord.RichEmbed()
            .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`)
            
            me.channel.send(brodeembed).then(async ll => {
                me.guild.members.forEach( m => {
           if(m.id != client.user.id && !m.user.bot)m.send(`${args}\n ${m}`).then(()=>{
            ll.edit(new Discord.RichEmbed()
            .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
        number1++
                        }).catch(function(){
                            errornumber1++
                            ll.edit(new Discord.RichEmbed()
                            .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n **فشل ارسال الى \`${errornumber1}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                        });
                    
             })
            })
           
            
            };    
            if (me.content.startsWith(prefix+"setname3")) {
              if(!args) return me.reply(`**${prefix}setname3 [name]**`)
            await client4.user.setUsername(args)
            me.channel.send(`تم تغير اسم الى ${args}`)
            }
            if (me.content.startsWith(prefix+"setavt3")) {
              if(!args) return me.reply(`**${prefix}setavt3 [avatar URL]**`)
              client4.user.setAvatar(args).then(
                me.channel.send(new Discord.RichEmbed().setTitle('تم تغير صورة الى').setThumbnail(args)).catch(error => {
                  return me.channel.send(error)
                 })  
              )
            }
                
                    
                                    
                                  });
                                  client5.on("message", async me => {
                                   
                                    if(!owners.includes(me.author.id)) return;
                                    let errornumber = 1
                                    
            
                                    if (!me.guild) return;
                                        let args = me.content.split(" ").slice(1).join(" ");
                                        if (me.content.startsWith(prefix + "obc4")) { 
                                     if(!args) return me.reply(new Discord.RichEmbed()
                                    .addField(`Online Boardcat`,`${prefix}obc1 [message]`))
                                    let number = 1
                                    let brodeembed = new Discord.RichEmbed()
                                    .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`)
                                    
                                    me.channel.send(brodeembed).then(async ll => { 
                                        
                                        
                                    await  me.guild.members.filter(m => m.presence.status !== 'offline').forEach( async m => {
                                      if(m.id != client.user.id && !m.user.bot)
                                      
                                      await m.send(`${args}\n ${m}`).then(()=>{
                                         ll.edit(new Discord.RichEmbed()
                                         .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
                                    number++
                                   
                                                    }).catch(function(){
                                                        errornumber++
                                                        ll.edit(new Discord.RichEmbed()
                                                        .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n **فشل ارسال الى \`${errornumber}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                                                    })
                                      })})
                                                   
                                    
                                      
                                      }
                                      if (!me.guild) return;
                          if (me.content.startsWith(prefix+"bc4")) {
            let number1 = 0
            let errornumber1 = 1
            
            let number02 = 0
                if(!args) return me.reply(new Discord.RichEmbed()
                .addField(`Boardcat to all`,`${prefix}bc1 [message]`));
                let brodeembed = new Discord.RichEmbed()
                .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`)
                
                me.channel.send(brodeembed).then(async ll => {
                    me.guild.members.forEach( m => {
               if(m.id != client.user.id && !m.user.bot)m.send(`${args}\n ${m}`).then(()=>{
                ll.edit(new Discord.RichEmbed()
                .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
            number1++
                            }).catch(function(){
                                errornumber1++
                                ll.edit(new Discord.RichEmbed()
                                .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n **فشل ارسال الى \`${errornumber1}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                            });
                        
                 })
                })
               
                
                };   
                if (me.content.startsWith(prefix+"setname4")) {
                  if(!args) return me.reply(`**${prefix}setname4 [name]**`)
                await client5.user.setUsername(args)
                me.channel.send(`تم تغير اسم الى ${args}`)
                }
                if (me.content.startsWith(prefix+"setavt4")) {
                  if(!args) return me.reply(`**${prefix}setavt4 [avatar URL]**`)
                  client5.user.setAvatar(args).then(
                    me.channel.send(new Discord.RichEmbed().setTitle('تم تغير صورة الى').setThumbnail(args)).catch(error => {
                      return me.channel.send(error)
                     })  
                  )
                } 
                        
                        
                                        
                                      });
                                      client6.on("message", async me => {
                                        if(!owners.includes(me.author.id)) return;
                                        let errornumber = 1
                                        
                
                                        if (!me.guild) return;
                                            let args = me.content.split(" ").slice(1).join(" ");
                                            if (me.content.startsWith(prefix + "obc5")) { 
                                         if(!args) return me.reply(new Discord.RichEmbed()
                                        .addField(`Online Boardcat`,`${prefix}obc1 [message]`))
                                        let number = 1
                                        let brodeembed = new Discord.RichEmbed()
                                        .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`)
                                        
                                        me.channel.send(brodeembed).then(async ll => { 
                                            
                                            
                                        await  me.guild.members.filter(m => m.presence.status !== 'offline').forEach( async m => {
                                          if(m.id != client.user.id && !m.user.bot)
                                          
                                          await m.send(`${args}\n ${m}`).then(()=>{
                                             ll.edit(new Discord.RichEmbed()
                                             .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
                                        number++
                                       
                                                        }).catch(function(){
                                                            errornumber++
                                                            ll.edit(new Discord.RichEmbed()
                                                            .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n **فشل ارسال الى \`${errornumber}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                                                        })
                                          })})
                                                       
                                        
                                          
                                          }
                                          if (!me.guild) return;
                              if (me.content.startsWith(prefix+"bc5")) {
                let number1 = 0
                let errornumber1 = 1
                
                let number02 = 0
                    if(!args) return me.reply(new Discord.RichEmbed()
                    .addField(`Boardcat to all`,`${prefix}bc1 [message]`));
                    let brodeembed = new Discord.RichEmbed()
                    .setDescription(`**تم ارسال بنجاح الى \`${number1}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`)
                    
                    me.channel.send(brodeembed).then(async ll => {
                        me.guild.members.forEach( m => {
                   if(m.id != client.user.id && !m.user.bot)m.send(`${args}\n ${m}`).then(()=>{
                    ll.edit(new Discord.RichEmbed()
                    .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n ** فشل ارسال الى \`${errornumber1}\` **`).addField(`**اخر شخص تم ارسال له:**`, m).setColor('GREEN').setFooter(me.guild.name, me.guild.iconURL)/*.setAuthor(me.author.username, me.author.avatarURL()).setTimestamp()*/)
                number1++
                                }).catch(function(){
                                    errornumber1++
                                    ll.edit(new Discord.RichEmbed()
                                    .setDescription(`**تم ارسال بنجاح الى \`${number}\`** \n **فشل ارسال الى \`${errornumber1}\`**`).addField(`اخر شخص ماقدرت ارسل له`, m).setColor('RED'))
                                });
                            
                     })
                    })
                    if (me.content.startsWith(prefix+"setname5")) {
                      if(!args) return me.reply(`**${prefix}setname5 [name]**`)
                    await client6.user.setUsername(args)
                    me.channel.send(`تم تغير اسم الى ${args}`)
                    }
                    if (me.content.startsWith(prefix+"setavt5")) {
                      if(!args) return me.reply(`**${prefix}setavt5 [avatar URL]**`)
                      client6.user.setAvatar(args).then(
                        me.channel.send(new Discord.RichEmbed().setTitle('تم تغير صورة الى').setThumbnail(args)).catch(error => {
                          return me.channel.send(error)
                         })  
                      )
                    }
                    
                    };    
                                            
                                          });
                        

                                          





client.login(process.env.token);

