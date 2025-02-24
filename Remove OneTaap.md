# --- [English] ---
🔹 **Simple but effective code to remove OneTap in your server**, making headshot damage the same as body damage.  

### 📌 **How to Use:**  
Add this code at the end of **qb-weapons\client\main.lua**  

### 🚀 **Code:**  
```lua
CreateThread(function()
    while true do
        Wait(0)
        local playerPed = PlayerPedId()
        local veh = GetVehiclePedIsIn(playerPed, false)
        if veh == 0 then
            SetPedSuffersCriticalHits(playerPed, false)
        end
    end
end)
```
✨ Now, any player who is not inside a vehicle **won't take extra headshot damage!**  
Enjoy your server without OneTap!

# --- [Arabic] ---
* هنا كود بسيط لكن فعّال لإزالة الـ OneTap في السيرفر، بحيث يكون الـ Damage للـ Head نفس الـ Body. 

### 📌 **طريقة الاستخدام:**
ضيف الكود ده في آخر **qb-weapons\client\main.lua**  

### 🚀 **الكود:**
```lua
CreateThread(function()
    while true do
        Wait(0)
        local playerPed = PlayerPedId()
        local veh = GetVehiclePedIsIn(playerPed, false)
        if veh == 0 then
            SetPedSuffersCriticalHits(playerPed, false)
        end
    end
end)
```
* كده أي حد مش راكب عربية مش هيتأثر بـ Headshot زيادة عن اللزوم!  
استمتع بالسيرفر بتاعك بدون OneTap!

# ---[CopyRights]---

- Author : i.dx#0
- Discord Link : https://discord.gg/b4s
