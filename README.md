# Emojify
An c# extention to be used for discord bot.


### Getting Started

None Embeds Way
```csharp
await Context.Channel.SendMessageAsync($"{Emojify.Smile} Hi");
```
Embeded Way
```C#
[Command("emojify")]
[Description("emoji class extention test")]
public async Task EmbedAsync() //string? You need to be using c# 8.0 or higher to use.
{
var embed = new EmbedBuilder():
embed.WithAuthor(Context.Author.Username);
embed.WithDescription($"{Emojify.Wave} Hello {Emojify.Grin}"):
await Context.Channel.SendMessageAsync(embed: embed.Build());
}
```
