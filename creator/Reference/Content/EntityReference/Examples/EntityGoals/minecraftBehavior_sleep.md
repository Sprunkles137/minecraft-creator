---
author: v-josjones
ms.author: v-josjones
title: Entity Documentation - minecraft:behavior.sleep
ms.prod: gaming
---

# Entity Documentation - minecraft:behavior.sleep

`minecraft:behavior.sleep` allows an entity to sleep in a bed.

> [!NOTE]
> This behavior can only be used by the `villager` entity type.

## Parameters

|Name |Default Value  |Type  |Description  |
|:----------|:----------|:----------|:----------|
|cooldown_time| 0.0| Decimal| Time in seconds the mob has to wait before using the goal again |
|sleep_collider_height| 1.0| Decimal|  The height of the mob's collider while sleeping |
|sleep_collider_width| 1.0| Decimal|  The width of the mob's collider while sleeping |
|sleep_y_offset| 1.0| Decimal|  The y offset of the mob's collider while sleeping |
|speed_multiplier| 1.0| Decimal|  Movement speed multiplier of the mob when using this AI Goal |
| timeout_cooldown| 8.0| Decimal| The cooldown time in seconds before the goal can be reused after a internal failure or timeout condition |

## Example

```json
"minecraft:behavior.sleep":{
    "priority": 2,
    "cooldown_time": 0.0,
    "sleep_collider_height": 1.0,
    "sleep_collider_width": 1.0,
    "sleep_y_offset": 1.0,
    "speed_multiplier": 1.0,
    "timer_cooldown": 8.0
}
```

## Vanilla entities examples

### villager_v2

:::code language="json" source="../../../../Source/VanillaBehaviorPack/entities/villager_v2.json" range="545-553":::

## Vanilla entities using `minecraft:behavior.sleep`

- [villager_v2](../../../../Source/VanillaBehaviorPack_Snippets/entities/villager_v2.md)
