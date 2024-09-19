---
sidebar_position: 1
---

# НИП (создать)
Создать НИПа
![npc.create](npcreate.uertyk.docs0001.png "By uertyk_ (unresoled of offical)")

---

Давайте творить пустышек!

:::warning ERROR - No_information
Доки все еще в разработке , ожидайте обновлений..!
:::

```kotlin
// Базовый НИП
val npc by NPCEntity.creating{
  // name = "Николай"
  pos = pos(0, -57, 0) // Если будет pos(<int>, <double>, <int>) - работать не будет
}
```

---
