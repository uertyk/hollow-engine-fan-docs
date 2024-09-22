---
sidebar_position: 1
---

# НИП (создать)
Создать НИПа
![npc.create](npcreate.uertyk.docs0001.png "by uertyk_ (unresoled of ofi)")

---

Давайте творить пустышек!

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# Скрипты (ЭТО НЕ ПРИМЕР):

<Tabs>
  <TabItem value="npc" label="Базовый НИП" default>
    ```kotlin
        val npc_id by NPCEntity.creating{
            // name = "npc_name"
            pos = pos(x, y, z) // позиция в мире
        }
    ```
  </TabItem>
  <TabItem value="anpc" label="Advenced НИП">
    ```kotlin
        val npc_id by NPCEntity.creating {
	        name = "npc_name" // имя
	        model = "path/to/model.gltf" // модель
	        animations[AnimationType.IDLE] = "defAnim.walk" // тип анимации (проигрывание/плавность)
	        transform = Transform(
		        sX = xf, sY = xf, sZ = xf // трансформация
	        )
	        pos = pos(x, y, z) // позиция в мире
        }
    ```
  </TabItem>
</Tabs>

# Скприпты (УЖЕ ПРИМЕР):

<Tabs>
  <TabItem value="npc" label="Базовый НИП" default>
    ```kotlin
        val yournpc by NPCEntity.creating{
            // name = "Твой НИП"
            pos = pos(52, -52, 52)
        }
    ```
  </TabItem>
  <TabItem value="anpc" label="Advenced НИП">
    ```kotlin
        val yournpc by NPCEntity.creating {
	        name = "Твой КрУтОй НИП"
	        model = "models:test.gltf"
	        // animations[AnimationType.IDLE] = "defAnim.walk" -- (хз как оно робит)
	        transform = Transform(
		        sX = 2f, sY = 2f, sZ = 2f
	        )
	        pos = pos(1488, -1488, 1488)
        }
    ```
  </TabItem>
</Tabs>
---
