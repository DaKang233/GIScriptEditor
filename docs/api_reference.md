# GIScript API Reference

本文件从 `GIScriptEditor/compiler.cpp` 中的 `Register(...)` 调用提取生成，覆盖 `FunctionRegistry` 与 `EventRegistry`。

说明：函数注册表只保存参数类型，不保存参数语义名称；函数参数名称因此按出现顺序标记为 `param1`、`param2` 等。事件注册表包含源码中的参数名称。重载项会以相同标题重复列出。

# 实体

## SetPresetStatus

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int

## GetPresetStatus

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Int

## DestroyEntity

返回值：

* void

参数：

1. param1 : Entity

## CreateEntity

返回值：

* void

参数：

1. param1 : EntityGuid
2. param2 : List<Int>

## GetSelfEntity

返回值：

* Entity

参数：

* 无

## QueryEntitybyGUID

返回值：

* Entity

参数：

1. param1 : EntityGuid

## QueryGUIDbyEntity

返回值：

* EntityGuid

参数：

1. param1 : Entity

## AddUniformBasicLinearMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String
3. param3 : Float
4. param4 : Vec

## AddUniformBasicRotationBasedMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String
3. param3 : Float
4. param4 : Float
5. param5 : Vec

## StopandDeleteBasicMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String
3. param3 : Bool

## PauseBasicMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## RecoverBasicMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## ActivateDisableCollisionTrigger

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Bool

## ActivateDisableEntityDeploymentGroup

返回值：

* void

参数：

1. param1 : Int
2. param2 : Bool

## GetCurrentlyActiveEntityDeploymentGroups

返回值：

* List<Int>

参数：

* 无

## Create3DVector

返回值：

* Vec

参数：

1. param1 : Float
2. param2 : Float
3. param3 : Float

## ActivateDisableNativeCollision

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## ActivateDisableNativeCollisionClimbability

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## ActivateDisableExtraCollision

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Bool

## ActivateDisableExtraCollisionClimbability

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Bool

## SwitchFollowMotionDeviceTargetbyGUID

返回值：

* void

参数：

1. param1 : Entity
2. param2 : EntityGuid
3. param3 : String
4. param4 : Vec
5. param5 : Vec

## GetListofPlayerEntitiesontheField

返回值：

* List<Entity>

参数：

* 无

## CreatePrefab

返回值：

* Entity

参数：

1. param1 : Prefab
2. param2 : Vec
3. param3 : Vec
4. param4 : Entity
5. param5 : Entity
6. param6 : Bool
7. param7 : Int
8. param8 : List<Int>

## CreateProjectile

返回值：

* Entity

参数：

1. param1 : Prefab
2. param2 : Vec
3. param3 : Vec
4. param4 : Entity
5. param5 : Entity
6. param6 : Bool
7. param7 : Int
8. param8 : List<Int>

## GetAllCharacterEntitiesofSpecifiedPlayer

返回值：

* List<Entity>

参数：

1. param1 : Entity

## GetPlayerEntitytoWhichtheCharacterBelongs

返回值：

* Entity

参数：

1. param1 : Entity

## GetEntityType

返回值：

* void

参数：

1. param1 : Entity

## ActivateBasicMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## GetPresetPointListbyUnitTag

返回值：

* List<Int>

参数：

1. param1 : Int

## DefeatAllPlayersCharacters

返回值：

* void

参数：

1. param1 : Entity

## TeleportPlayer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Vec
3. param3 : Vec

## GetEntitiesWithSpecifiedPrefabontheField

返回值：

* List<Entity>

参数：

1. param1 : Prefab

## RemoveEntity

返回值：

* void

参数：

1. param1 : Entity

## GetCreationsCurrentTarget

返回值：

* Entity

参数：

1. param1 : Entity

## GetEntityListbySpecifiedType

返回值：

* List<Entity>

参数：

1. param1 : List<Entity>

## GetEntityListbySpecifiedPrefab

返回值：

* List<Entity>

参数：

1. param1 : List<Entity>
2. param2 : Prefab

## GetEntityListbySpecifiedRange

返回值：

* List<Entity>

参数：

1. param1 : List<Entity>
2. param2 : Vec
3. param3 : Float

## QueryPlayerClass

返回值：

* Config

参数：

1. param1 : Entity

## QueryPlayerClassLevel

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Config

## ChangePlayerClass

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## IncreasePlayersCurrentClassEXP

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ChangePlayersCurrentClassLevel

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## QueryIfEntityIsontheField

返回值：

* Bool

参数：

1. param1 : Entity

## GetEntityForwardVector

返回值：

* Vec

参数：

1. param1 : Entity

## GetEntityRightVector

返回值：

* Vec

参数：

1. param1 : Entity

## GetEntityUpwardVector

返回值：

* Vec

参数：

1. param1 : Entity

## DirectionVectortoRotation

返回值：

* Vec

参数：

1. param1 : Vec
2. param2 : Vec

## AddTargetOrientedRotationBasedMotionDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String
3. param3 : Float
4. param4 : Vec

## AddUnitTagtoEntity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## RemoveUnitTagfromEntity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ClearUnitTagsfromEntity

返回值：

* void

参数：

1. param1 : Entity

## GetEntityUnitTagList

返回值：

* List<Int>

参数：

1. param1 : Entity

## GetEntityListbyUnitTag

返回值：

* List<Entity>

参数：

1. param1 : Int

## AddEntityActiveNameplate

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## DeleteEntityActiveNameplate

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## SetEntityActiveNameplate

返回值：

* void

参数：

1. param1 : Entity
2. param2 : List<Config>

## SwitchCreationPatrolTemplate

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ToggleEntityLightSource

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Bool

## SwitchFollowMotionDeviceTargetByEntity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Entity
3. param3 : String
4. param4 : Vec
5. param5 : Vec

## GetAllEntitiesWithinTheCollisionTrigger

返回值：

* List<Entity>

参数：

1. param1 : Entity
2. param2 : Int

## GetOwnerEntity

返回值：

* Entity

参数：

1. param1 : Entity

## GetListOfEntitiesOwnedByTheEntity

返回值：

* List<Entity>

参数：

1. param1 : Entity

## GetPlayerGUIDbyPlayerID

返回值：

* EntityGuid

参数：

1. param1 : Int

## GetPlayerIDbyPlayerGUID

返回值：

* Int

参数：

1. param1 : EntityGuid

## CreatePrefabGroup

返回值：

* List<Entity>

参数：

1. param1 : Int
2. param2 : Vec
3. param3 : Vec
4. param4 : Entity
5. param5 : Entity
6. param6 : Int
7. param7 : List<Int>
8. param8 : Bool

## QueryGameModeAndPlayerNumber

返回值：

* Int

参数：

* 无

## GetPlayerNickname

返回值：

* String

参数：

1. param1 : Entity

## GetPlayerClientInputDeviceType

返回值：

* void

参数：

1. param1 : Entity

## ModifyPlayerChannelPermission

返回值：

* void

参数：

1. param1 : EntityGuid
2. param2 : Int
3. param3 : Bool

## SetPlayersCurrentChannel

返回值：

* void

参数：

1. param1 : EntityGuid
2. param2 : List<Int>

# 计时器

## StartTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String
3. param3 : Bool
4. param4 : List<Float>

## PauseTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## ResumeTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## StopTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## PlayTimedEffects

返回值：

* void

参数：

1. param1 : Config
2. param2 : Entity
3. param3 : String
4. param4 : Bool
5. param5 : Bool
6. param6 : Vec
7. param7 : Vec
8. param8 : Float
9. param9 : Bool

## GetPlayerReviveTime

返回值：

* Int

参数：

1. param1 : Entity

## SetPlayerReviveTime

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## QueryGameTimeElapsed

返回值：

* Int

参数：

* 无

## PauseGlobalTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## GetCurrentGlobalTimerTime

返回值：

* Float

参数：

1. param1 : Entity
2. param2 : String

## StartGlobalTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## RecoverGlobalTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## StopGlobalTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String

## ModifyGlobalTimer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : String
3. param3 : Float

## SetCurrentEnvironmentTime

返回值：

* void

参数：

1. param1 : Float

## SetEnvironmentTimePassageSpeed

返回值：

* void

参数：

1. param1 : Float

## CalculateTimestampFromFormattedTime

返回值：

* Int

参数：

1. param1 : Int
2. param2 : Int
3. param3 : Int
4. param4 : Int
5. param5 : Int
6. param6 : Int

## Calculatedayoftheweekfromtimestamp

返回值：

* Int

参数：

1. param1 : Int

## QueryTimestampUTC0

返回值：

* Int

参数：

* 无

## QueryServerTimeZone

返回值：

* Int

参数：

* 无

# 战斗

## QueryEntityFaction

返回值：

* Faction

参数：

1. param1 : Entity

## ModifyEntityFaction

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Faction

## ActivateRevivePoint

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## DeactivateRevivePoint

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## AllowForbidPlayertoRevive

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## GetPlayerRemainingRevives

返回值：

* Int

参数：

1. param1 : Entity

## SetPlayerRemainingRevives

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ReviveCharacter

返回值：

* void

参数：

1. param1 : Entity

## ReviveAllPlayersCharacters

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## QueryIfAllPlayerCharactersAreDown

返回值：

* Bool

参数：

1. param1 : Entity

## ModifyingCharacterDisruptorDevice

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## InitiateAttack

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Float
3. param3 : Float
4. param4 : Vec
5. param5 : Vec
6. param6 : String
7. param7 : Bool
8. param8 : Entity

## GetEntityListbySpecifiedFaction

返回值：

* List<Entity>

参数：

1. param1 : List<Entity>
2. param2 : Faction

## ModifySkillResourceAmount

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Float

## SetSkillResourceAmount

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Float

## AddCharacterSkill

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## DeleteCharacterSkillbyID

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## InitializeCharacterSkill

返回值：

* void

参数：

1. param1 : Entity

## QueryCharacterSkill

返回值：

* Config

参数：

1. param1 : Entity

## DeleteCharacterSkillbySlot

返回值：

* void

参数：

1. param1 : Entity

## QueryIfEntityHasUnitStatus

返回值：

* Bool

参数：

1. param1 : Entity
2. param2 : Config

## RecoverHP

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Float
3. param3 : String
4. param4 : Bool
5. param5 : Entity

## QueryifSpecifiedEntityIsinCombat

返回值：

* Bool

参数：

1. param1 : Entity

## QueryIfFactionIsHostile

返回值：

* Bool

参数：

1. param1 : Faction
2. param2 : Faction

## HPLoss

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Float
3. param3 : Bool
4. param4 : Bool
5. param5 : Bool

## RecoverHPDirectly

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Entity
3. param3 : Float
4. param4 : Bool
5. param5 : Float
6. param6 : Float
7. param7 : List<String>

## QueryUnitStatusStacksBySlotID

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## QueryUnitStatusApplierBySlotID

返回值：

* Entity

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## ListOfSlotIDsQueryingUnitStatus

返回值：

* List<Int>

参数：

1. param1 : Entity
2. param2 : Config

# UI

## SwitchMainCameraTemplate

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : String

## ActivateEntityCamera

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : Entity

## DisableEntityCamera

返回值：

* void

参数：

1. param1 : List<Entity>

## ActivateFocusCamera

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : Entity

## DisableFocusCamera

返回值：

* void

参数：

1. param1 : List<Entity>

## ActivateScreenShake

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : Float
3. param3 : Float
4. param4 : Float

## ActivateDisableTab

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Bool

## GetPlayersCurrentUILayout

返回值：

* Int

参数：

1. param1 : Entity

## SwitchCurrentInterfaceLayout

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ActivateUIControlGroupinControlGroupLibrary

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ModifyUIControlStatusWithintheInterfaceLayout

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## RemoveInterfaceControlGroupFromControlGroupLibrary

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## CloseSpecifiedSoundEffectPlayer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## StartPauseSpecifiedSoundEffectPlayer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Bool

## AdjustSpecifiedSoundEffectPlayer

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int
4. param4 : Float

## StartPausePlayerBackgroundMusic

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## AdjustPlayerBackgroundMusicVolume

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ModifyPlayerBackgroundMusic

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Float
4. param4 : Float
5. param5 : Int
6. param6 : Bool
7. param7 : Float
8. param8 : Float
9. param9 : Bool

## PlayerPlaysOneShot2DSoundEffect

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int
4. param4 : Float

## SwitchActiveTextBubble

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## ModifyMiniMapZoom

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Float

## ModifyMiniMapMarkerActivationStatus

返回值：

* void

参数：

1. param1 : Entity
2. param2 : List<Int>
3. param3 : Bool

## ModifyPlayerListforVisibleMiniMapMarkers

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : List<Entity>

## ModifyPlayerListforTrackingMiniMapMarkers

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : List<Entity>

## ModifyPlayerMarkersontheMiniMap

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Entity

## QueryIfAchievementIsCompleted

返回值：

* Bool

参数：

1. param1 : Entity
2. param2 : Int

## SetAchievementProgressTally

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int

## ChangeAchievementProgressTally

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int

## SetPlayerSettlementRankingValue

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## GetPlayerSettlementRankingValue

返回值：

* Int

参数：

1. param1 : Entity

## SetPlayerSettlementSuccessStatus

返回值：

* void

参数：

1. param1 : Entity

## GetPlayerSettlementSuccessStatus

返回值：

* void

参数：

1. param1 : Entity

## SetFactionSettlementRankingValue

返回值：

* void

参数：

1. param1 : Faction
2. param2 : Int

## GetFactionSettlementRankingValue

返回值：

* Int

参数：

1. param1 : Faction

## SetFactionSettlementSuccessStatus

返回值：

* void

参数：

1. param1 : Faction

## GetFactionSettlementSuccessStatus

返回值：

* void

参数：

1. param1 : Faction

## GetPlayerRankScoreChange

返回值：

* Int

参数：

1. param1 : Entity

## SetPlayerEscapeValidity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## GetPlayerEscapeValidity

返回值：

* Bool

参数：

1. param1 : Entity

## Switchthescoringgroupthataffectsplayerscompetitiverank

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## UpdatePlayerLeaderboardScore

返回值：

* void

参数：

1. param1 : List<Int>
2. param2 : Int
3. param3 : Int

## SetPlayerLeaderboardScoreAsan

返回值：

* void

参数：

1. param1 : List<Int>
2. param2 : Int
3. param3 : Int

## SetPlayerLeaderboardScoreAsan

返回值：

* void

参数：

1. param1 : List<Int>
2. param2 : Float
3. param3 : Int

## SetChatChannelSwitch

返回值：

* void

参数：

1. param1 : Int
2. param2 : Bool
3. param3 : Bool

# 商店

## AddAffixToEquipment

返回值：

* void

参数：

1. param1 : Int
2. param2 : Config
3. param3 : Bool
4. param4 : Float

## RemoveEquipmentAffix

返回值：

* void

参数：

1. param1 : Int
2. param2 : Int

## ModifyEquipmentAffixValue

返回值：

* void

参数：

1. param1 : Int
2. param2 : Int
3. param3 : Float

## GetEquipmentAffixList

返回值：

* List<Int>

参数：

1. param1 : Int

## GetEquipmentAffixConfigID

返回值：

* Config

参数：

1. param1 : Int
2. param2 : Int

## GetEquipmentAffixValue

返回值：

* Float

参数：

1. param1 : Int
2. param2 : Int

## IncreaseMaximumInventoryCapacity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## ModifyInventoryItemQuantity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## SetInventoryDropItemsCurrencyAmount

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## ModifyInventoryCurrencyQuantity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## GetInventoryCapacity

返回值：

* Int

参数：

1. param1 : Entity

## GetInventoryItemQuantity

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Config

## GetInventoryCurrencyQuantity

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Config

## OpenShop

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Entity
3. param3 : Int

## CloseShop

返回值：

* void

参数：

1. param1 : Entity

## RemoveItemFromCustomShopSalesList

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int

## RemoveItemFromInventoryShopSalesList

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Config

## RemoveItemFromPurchaseList

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Config

## QueryCustomShopItemSalesList

返回值：

* List<Int>

参数：

1. param1 : Entity
2. param2 : Int

## QueryInventoryShopItemSalesList

返回值：

* List<Config>

参数：

1. param1 : Entity
2. param2 : Int

## QueryShopPurchaseItemList

返回值：

* List<Config>

参数：

1. param1 : Entity
2. param2 : Int

## GetAllEquipmentFromInventory

返回值：

* List<Int>

参数：

1. param1 : Entity

## SetLootDropContent

返回值：

* void

参数：

1. param1 : Entity

## ModifyLootItemComponentQuantity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## ModifyLootComponentCurrencyAmount

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config
3. param3 : Int

## GetLootComponentItemQuantity

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Config

## GetLootComponentCurrencyQuantity

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Config

## GetAllTrophyItems

返回值：

* void

参数：

1. param1 : Entity

## GetAllTrophyCurrency

返回值：

* void

参数：

1. param1 : Entity

## GetAllEquipmentFromLootComponent

返回值：

* List<Int>

参数：

1. param1 : Entity

## QueryEquipmentTagList

返回值：

* List<Config>

参数：

1. param1 : Int

## AddAffixToEquipmentAtSpecifiedID

返回值：

* void

参数：

1. param1 : Int
2. param2 : Config
3. param3 : Int
4. param4 : Bool
5. param5 : Float

## QueryEquipmentConfigIDbyEquipmentID

返回值：

* Config

参数：

1. param1 : Int

## ConsumeGiftBox

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int
3. param3 : Int

## QueryCorrespondingGiftBoxQuantity

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Int

## QueryCorrespondingGiftBoxConsumption

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Int

# 仇恨系统

## SettheAggroValueofSpecifiedEntity

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Entity
3. param3 : Int

## RemoveTargetEntityFromAggroList

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Entity

## ClearSpecifiedTargetsAggroList

返回值：

* void

参数：

1. param1 : Entity

## TauntTarget

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Entity

## QuerytheAggroValueoftheSpecifiedEntity

返回值：

* Int

参数：

1. param1 : Entity
2. param2 : Entity

## QuerytheAggroMultiplieroftheSpecifiedEntity

返回值：

* Float

参数：

1. param1 : Entity

## QueryGlobalAggroTransferMultiplier

返回值：

* Float

参数：

* 无

## GettheAggroTargetoftheSpecifiedEntity

返回值：

* Entity

参数：

1. param1 : Entity

## GetListofOwnersWhoHavetheTargetinTheirAggroList

返回值：

* List<Entity>

参数：

1. param1 : Entity

## GetListofOwnersThatHavetheTargetAsTheirAggroTarget

返回值：

* List<Entity>

参数：

1. param1 : Entity

## GettheAggroListoftheSpecifiedEntity

返回值：

* List<Entity>

参数：

1. param1 : Entity

## GetAggroListOfCreationInDefaultMode

返回值：

* List<Entity>

参数：

1. param1 : Entity

# 其他

## print

返回值：

* void

参数：

1. param1 : String

## ForwardEvent

返回值：

* void

参数：

1. param1 : Entity

## GetRandomFloatingPointNumber

返回值：

* Float

参数：

1. param1 : Float
2. param2 : Float

## WeightedRandom

返回值：

* Int

参数：

1. param1 : List<Int>

## SettleStage

返回值：

* void

参数：

1. param1 : Bool

## MountLoopingSpecialEffect

返回值：

* Int

参数：

1. param1 : Config
2. param2 : Entity
3. param3 : String
4. param4 : Bool
5. param5 : Bool
6. param6 : Vec
7. param7 : Vec
8. param8 : Float
9. param9 : Bool

## ClearLoopingSpecialEffect

返回值：

* void

参数：

1. param1 : Int
2. param2 : Entity

## ForwardingEvent

返回值：

* void

参数：

1. param1 : Entity

## Pi

返回值：

* Float

参数：

1. param1 : Float

## ModuloOperation

返回值：

* Int

参数：

1. param1 : Int
2. param2 : Int

## LogarithmOperation

返回值：

* Float

参数：

1. param1 : Float
2. param2 : Float

## ArithmeticSquareRootOperation

返回值：

* Float

参数：

1. param1 : Float

## RoundtoIntegerOperation

返回值：

* Int

参数：

1. param1 : Float

## LogicalANDOperation

返回值：

* Bool

参数：

1. param1 : Bool
2. param2 : Bool

## LogicalOROperation

返回值：

* Bool

参数：

1. param1 : Bool
2. param2 : Bool

## LogicalXOROperation

返回值：

* Bool

参数：

1. param1 : Bool
2. param2 : Bool

## LogicalNOTOperation

返回值：

* Bool

参数：

1. param1 : Bool
2. param2 : Bool

## DistanceBetweenTwoCoordinatePoints

返回值：

* Float

参数：

1. param1 : Vec
2. param2 : Vec

## GetRandomInteger

返回值：

* Int

参数：

1. param1 : Int
2. param2 : Int

## SineFunction

返回值：

* Float

参数：

1. param1 : Float

## CosineFunction

返回值：

* Float

参数：

1. param1 : Float

## TangentFunction

返回值：

* Float

参数：

1. param1 : Float

## ArcsineFunction

返回值：

* Float

参数：

1. param1 : Float

## ArccosineFunction

返回值：

* Float

参数：

1. param1 : Float

## ArctangentFunction

返回值：

* Float

参数：

1. param1 : Float

## ActivateDisableModelDisplay

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Bool

## GetAllEntitiesontheField

返回值：

* List<Entity>

参数：

* 无

## GetSpecifiedTypeofEntitiesontheField

返回值：

* List<Entity>

参数：

* 无

## RadianstoDegrees

返回值：

* Float

参数：

1. param1 : Float

## DegreestoRadians

返回值：

* Float

参数：

1. param1 : Float

## ClearSpecialEffectsBasedonSpecialEffectAssets

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Config

## CloseDeckSelector

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## SetScanTagRules

返回值：

* void

参数：

1. param1 : Entity

## SetScanComponentsActiveScanTagID

返回值：

* void

参数：

1. param1 : Entity
2. param2 : Int

## GetTheCurrentlyActiveScanTagConfigID

返回值：

* Config

参数：

1. param1 : Entity

## RandomDeckSelectorSelectionList

返回值：

* void

参数：

1. param1 : List<Int>

## ModifyEnvironmentSettings

返回值：

* void

参数：

1. param1 : Int
2. param2 : List<Entity>
3. param3 : Bool
4. param4 : Int

## WriteByBit

返回值：

* Int

参数：

1. param1 : Int
2. param2 : Int
3. param3 : Int
4. param4 : Int

## ReadByBit

返回值：

* Int

参数：

1. param1 : Int
2. param2 : Int
3. param3 : Int

## InsertValue

返回值：

* void

参数：

1. param1 : List<Int>
2. param2 : Int
3. param3 : Int

## InsertValue

返回值：

* void

参数：

1. param1 : List<String>
2. param2 : Int
3. param3 : String

## InsertValue

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : Int
3. param3 : Entity

## InsertValue

返回值：

* void

参数：

1. param1 : List<EntityGuid>
2. param2 : Int
3. param3 : EntityGuid

## InsertValue

返回值：

* void

参数：

1. param1 : List<Float>
2. param2 : Int
3. param3 : Float

## InsertValue

返回值：

* void

参数：

1. param1 : List<Vec>
2. param2 : Int
3. param3 : Vec

## InsertValue

返回值：

* void

参数：

1. param1 : List<Bool>
2. param2 : Int
3. param3 : Bool

## InsertValue

返回值：

* void

参数：

1. param1 : List<Config>
2. param2 : Int
3. param3 : Config

## InsertValue

返回值：

* void

参数：

1. param1 : List<Prefab>
2. param2 : Int
3. param3 : Prefab

## InsertValue

返回值：

* void

参数：

1. param1 : List<Faction>
2. param2 : Int
3. param3 : Faction

## SetValue

返回值：

* void

参数：

1. param1 : List<Int>
2. param2 : Int
3. param3 : Int

## SetValue

返回值：

* void

参数：

1. param1 : List<String>
2. param2 : Int
3. param3 : String

## SetValue

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : Int
3. param3 : Entity

## SetValue

返回值：

* void

参数：

1. param1 : List<EntityGuid>
2. param2 : Int
3. param3 : EntityGuid

## SetValue

返回值：

* void

参数：

1. param1 : List<Float>
2. param2 : Int
3. param3 : Float

## SetValue

返回值：

* void

参数：

1. param1 : List<Vec>
2. param2 : Int
3. param3 : Vec

## SetValue

返回值：

* void

参数：

1. param1 : List<Bool>
2. param2 : Int
3. param3 : Bool

## SetValue

返回值：

* void

参数：

1. param1 : List<Config>
2. param2 : Int
3. param3 : Config

## SetValue

返回值：

* void

参数：

1. param1 : List<Prefab>
2. param2 : Int
3. param3 : Prefab

## SetValue

返回值：

* void

参数：

1. param1 : List<Faction>
2. param2 : Int
3. param3 : Faction

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Int>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<String>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Entity>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<EntityGuid>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Float>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Vec>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Bool>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Config>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Prefab>
2. param2 : Int

## RemoveValue

返回值：

* void

参数：

1. param1 : List<Faction>
2. param2 : Int

## Clear

返回值：

* void

参数：

1. param1 : List<Int>

## Clear

返回值：

* void

参数：

1. param1 : List<String>

## Clear

返回值：

* void

参数：

1. param1 : List<Entity>

## Clear

返回值：

* void

参数：

1. param1 : List<EntityGuid>

## Clear

返回值：

* void

参数：

1. param1 : List<Float>

## Clear

返回值：

* void

参数：

1. param1 : List<Vec>

## Clear

返回值：

* void

参数：

1. param1 : List<Bool>

## Clear

返回值：

* void

参数：

1. param1 : List<Config>

## Clear

返回值：

* void

参数：

1. param1 : List<Prefab>

## Clear

返回值：

* void

参数：

1. param1 : List<Faction>

# 事件

以下事件同样来自 `EventRegistry::Register(...)`；事件返回值统一为 `void`。

## 实体

### OnEntityCreated

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid

### OnEntityRemovedDestroyed

返回值：

* void

参数：

1. source : EntityGuid

### OnPresetStatusChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int
4. b : Int
5. c : Int

### OnBasicMotionDeviceStops

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : String

### OnExitingCollisionTrigger

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : EntityGuid
5. c : Int

### OnEnteringCollisionTrigger

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : EntityGuid
5. c : Int

### OnPlayerTeleportCompletes

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid

### OnPlayerClassChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Config

### OnPlayerClassLevelChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int
4. b : Int

### OnCreationReachesPatrolWaypoint

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int
4. b : Int
5. c : Int
6. d : Int

### OnPlayerClassIsRemoved

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Config

## 计时器

### OnTimerIsTriggered

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : String
4. b : Int
5. c : Int
6. d : EntityGuid

### OnGlobalTimerIsTriggered

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : String

## 战斗

### OnEntityFactionChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Faction
4. b : Faction

### OnOnHitDetectionIsTriggered

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Bool
4. b : Entity
5. c : Vec

### OnCharacterRevives

返回值：

* void

参数：

1. sourceEntity : Entity

### OnAllPlayersCharactersAreDown

返回值：

* void

参数：

1. sourceEntity : Entity

### OnPlayerIsAbnormallyDownedandRevives

返回值：

* void

参数：

1. sourceEntity : Entity

### OnAllPlayersCharactersAreRevived

返回值：

* void

参数：

1. sourceEntity : Entity

### OnUnitStatusChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Entity
5. c : Bool
6. d : Float
7. e : Int
8. f : Int
9. g : Int

### OnCreationEntersCombat

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid

### OnCreationLeavesCombat

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid

### OnSkillNodeIsCalled

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : String
4. b : String
5. c : String

### OnHPIsRecovered

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : Float
5. c : List<String>

### OnInitiatingHPRecovery

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : Float
5. c : List<String>

### OnSelfEntersCombat

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid

### OnSelfLeavesCombat

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid

### OnShieldIsAttacked

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : EntityGuid
5. c : Config
6. d : Int
7. e : Int
8. f : Float
9. g : Float

## UI

### OnTabIsSelected

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int
4. b : Entity
5. c : EntityGuid

### OnUIControlGroupIsTriggered

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int
4. b : Int

### OnTextBubbleIsCompleted

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : Entity
3. a : Config
4. b : Int

## 商店

### OnEquipmentAffixValueChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int
4. b : Int
5. c : Float
6. d : Float

### OnItemIsAddedtoInventory

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Int

### OnItemIsLostFromInventory

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Int

### OntheQuantityofInventoryItemChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Int
5. c : Int

### OntheQuantityofInventoryCurrencyChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Int

### OnEquipmentIsInitialized

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int

### OnEquipmentIsEquipped

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int

### OnEquipmentIsUnequipped

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Int

### OnCustomShopItemIsSold

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : Int
5. c : Int
6. d : Int

### OnSellingInventoryItemsintheShop

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : Int
5. c : Config
6. d : Int

### OnItemsintheInventoryAreUsed

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Config
4. b : Int

## 仇恨系统

### OnAggroTargetChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity
4. b : Entity

## 其他

### OnPathReachesWaypoint

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : String
4. b : Int
5. c : Int

### OnEnteringanInterruptibleState

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. a : Entity

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Int
5. after : Int

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : String
5. after : String

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Entity
5. after : Entity

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : EntityGuid
5. after : EntityGuid

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Float
5. after : Float

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Vec
5. after : Vec

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Bool
5. after : Bool

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Config
5. after : Config

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Prefab
5. after : Prefab

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : Faction
5. after : Faction

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Int>
5. after : List<Int>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<String>
5. after : List<String>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Entity>
5. after : List<Entity>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<EntityGuid>
5. after : List<EntityGuid>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Float>
5. after : List<Float>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Vec>
5. after : List<Vec>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Bool>
5. after : List<Bool>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Config>
5. after : List<Config>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Prefab>
5. after : List<Prefab>

### OnCustomVariableChanges

返回值：

* void

参数：

1. sourceEntity : Entity
2. sourceGuid : EntityGuid
3. name : String
4. before : List<Faction>
5. after : List<Faction>
