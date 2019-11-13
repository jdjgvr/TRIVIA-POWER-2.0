import discord
from discord.ext.commands import bot
from discord import game
from discord.ext import commands

client = commands.Bot(command_prefix = '%')

@client.event
async def on_ready():
    print('Logged in as '+client.user.name)
    print('--------')
@commands.has_permissions(administrator=True)
@client.command(pass_context = True)
async def send(ctx, *, content: str):
        for member in ctx.message.server.members:
            try:
                await client.send_message(member, content)
                await client.say("DM Sent To : {} :white_check_mark:  ".format(member))
            except:
                print("can't")
                await client.say("DM can't Sent To : {} :x: ".format(member))

client.run("NTk0ODk0NTE5NzAzNDM3MzIy.XRnCiA._hIcWEZKe2yocgWW3KM_4Xbj91Q")
  
