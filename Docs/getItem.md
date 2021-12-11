# getItem

Get item by name or id. 

### Usage

```js
client.eco.getItem(GuildID, item) 
```

### Example

```js


let data = await client.eco.GetInv(message.guild.id, 0) 

let embed = new MessageEmbed()
  .setTitle(`Item "${data.Name}"`)
  .addField("Price", data.Price.toString())
  .addField("Selling price", data.Sell.toString())
  .addField("ID", data.id.toString())
  .setTimestamp()

```

- ## Returns `Item` on success
 
```js
{ Name: string, Price: string, Sell: string, id: 0 | number };
```

 - ## Returns `null` on error - if no item in inv

 - ### Options

- no options ;(