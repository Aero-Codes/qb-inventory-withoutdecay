# Inventory Decay

![image](https://user-images.githubusercontent.com/80186604/163069477-114e14ec-bec1-4f93-8421-42017c605f15.png)

## Credits:
>### aj - aj-inventory
>### loljoshie - lj-inventory
>### qbcore - qb-inventory
>### Jimathy - Toggle Item

# How to install lj-inventory
* Download source files from github
* Drag source files into your resources folder
* Rename folder from `lj-inventory-main` to `lj-inventory`

### REPLACE
```lua
TriggerServerEvent("QBCore:Server:AddItem, item, 1)
```

### TO
```lua
exports['qb-inventory']:toggleItem(1, itemName, 1)
```

### REPLACE
```lua
TriggerServerEvent("QBCore:Server:RemoveItem, item, 1)
```

### TO
```lua
exports['qb-inventory']:toggleItem(0, itemName, 1)
```


### REPLACE
```lua
QBCore.Functions.HasItem("sandwich", function(hasitem)
        if hasitem then
              -- Has Item
        end
end)
```

### TO
```lua
      if QBCore.Functions.HasItem("sandwich") then
             -- Has Item
      end
```
