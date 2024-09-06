# 🚪 Door Ding - Interactive Delivery System 📦

Enhance your server with the ultimate delivery experience!

## 🌟 Overview

Introducing **Door Ding**: a cutting-edge solution designed to revolutionize your server's legal funding operations. With sophisticated scripting and intuitive functionality, Door Ding offers an immersive delivery experience perfect for role-playing servers.

## 🔥 Features

- **📱 Interactive HTML Tablet**: Players use the `/doording` command to access a fully functional HTML tablet, which serves as the hub for managing deliveries.
- **🎨 Customizable Settings**: Personalize the tablet experience with options to choose preferred languages and backgrounds via the settings button, boosting user engagement and accessibility.
- **🚚 Advanced Delivery Mechanics**: Enjoy real-time notifications for smooth handling of deliveries.
- **🎭 Realistic Animations**: Experience detailed animations for picking up and dropping off items, enhancing player interactions.
- **📋 Order Management**: Players can accept or decline orders with a system that tracks timers for pickup and drop-off. Set waypoints to guide your delivery route.
- **💵 Cash Tip System**: Receive tips from clients after completing deliveries, complete with a realistic cash exchange animation.
- **⏸️ Pause and Resume Functionality**: Flexibly manage in-game activities with support for pausing and resuming deliveries.

## 🛠️ Installation

1. Download the package from Keymaster.
2. Open and adjust `config.lua` to suit server needs.
3. Copy the package into the `resources` directory (or desired sub-directory).
4. Ensure the copied resource is listed in your `server.cfg`.

## 🚀 How to Use

1. Execute the command `doording` through F8 or `/doording` in chat.
2. Click "Start Dinging" (or the locale equivalent).
3. Accept an order.
4. Travel to the pickup location.
5. Walk to the front of the pickup worker.
6. Travel to the drop-off location.
7. Walk to the front of the drop-off client.
8. Wait for order completion.

## 🛡️ Support & Compatibility

Door Ding is standalone and can be configured for framework integration.

### Example: Inventory Integration with OX Inventory

Add the following to `ox_inventory/data/items.lua`:

```lua
['dingtablet'] = {
    label = 'Door Ding Tablet',
    weight = 100,
    client = {
        image = 'some_image.png',
    },
    buttons = {
        {
            label = 'Use',
            action = function(slot)
                ExecuteCommand("DoorDing")
            end
        },
    },
},
```

For support or customization requests, consult our readme files or contact our support team.

Transform your server’s delivery experience with Door Ding! Whether running a bustling city or a tight-knit community, our delivery system adds depth and realism to your gameplay. 🌆🚛