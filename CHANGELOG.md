# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2022-06-19
### Added
- SpongeAbsorbEvent.
- EntityArrowStuckEvent.
- PlayerAnvilDamageEvent.
- EntityMoveEvent.
- AnyEntitySpawnEvent.
- EntityTickEvent.
- TileEntityTickEvent.
- Depth API for the BlockPhysicsEvent.
- Silent "setTypeIdAndData" for the Block class.
- Added depencency "com.github.ben-manes.caffeine:caffeine:2.9.3".
- Velocity natives for encryption and compression.
- Dynamic player view distance.
- Delayed chunk send.
- Old combat system.
- Enhanced lighting queue.
- Configurable portal travel cache.
- Configurable wither spawn shape check.
- Configurable end portal shape check.
- Configurable nether portal shape check.
- Configurable halloween mob feature.
- Configurable Paper custom flow speed feature.
- Configurable step sounds.
- Configurable villagers.
- Configurable time update period.
- Configurable relative arrow motion.
- Configurable ping period.
- Round player ping.
- Entity tracker Y check.
- More timings.

### Changed
- Updated dependency "org.apache.commons:commons-lang3:3.12.0".
- Updated dependency "io.netty:netty-all:4.1.77.Final".
- Updated dependency "org.xerial:sqlite-jdbc:3.36.0.3".
- Updated dependency "mysql:mysql-connector-java:8.0.29".
- Updated dependency "it.unimi.dsi:fastutil:8.5.8".
- Reduced offline mode console warn.
- Increased max view distance from 32 to 64.
- Always full chat visibility.
- Optimized player lookup by name.
- Optimized physics update loop.
- Optimized block event queue.
- Don't reduntandtly call "toArray" in the Chunk "getEntities" and "getTileEntities" methods.
- Cache tamable entity owner.
- Cache "isInLava" entity check result.
- Cache current entity BlockPosition.
- Cache Spigot and Paper world configs.
- Reduced EntityTracker updates on "updatePotionMetadata".
- Reduced PlayerInventory updates.
- Lithium - ai/pathing/ChunkCache.
- Lithium - ai/pathing/LandPathNodeMaker.
- Lithium - math/sine_lut/MathHelper.
- Optimized chat component parsing.
- Optimized NetworkManager.
- Consolidate flush calls for entity tracker packets.
- Using "MethodHandle" instead of "Reflection" for instantiating "MaterialData".
- Don't tick "EnchantmentTable".
- Don't tick "EndGateway" when not in the end world.
- Guava cache replaced with Caffeine cache.
- Don't check "DataVersion" on chunk load.
- Don't reattach "RootVehicle" that too far on player data load.
- Cache chunk NBT in the PacketPlayOutMapChunk.
- Deactivated PooledBlockPosition.
- Micro-optimizations.

### Removed
- Paper Anti-Xray.
- Mojang snooper.
- Sign commands.

### Fixed
- [MC-101232](https://bugs.mojang.com/browse/MC-101232).
- [MC-103516](https://bugs.mojang.com/browse/MC-103516).
- [MC-120780](https://bugs.mojang.com/browse/MC-120780).
- [MC-128547](https://bugs.mojang.com/browse/MC-128547).
- Various Bukkit API fixes.
- PlayerInteractEvent not called in specific situations.
- Worlds not saving in specific situations.
- Don't send unreachable blocks [\[1\]](https://github.com/nerdsinspace/nocom-explanation/blob/main/README.md) [\[2\]](https://2b2t.miraheze.org/wiki/Nocom).
- TileEntity ticking crash.
- Don't save NaN entity positions.
- Player "setViewDistance" bug.
- Don't accept invalid client settings.
- Entity remount dupe [\[1\]](https://youtu.be/yi8SWMzk-og) [\[2\]](https://youtu.be/9-7KrUMXkv8).
- Entity ride desync dupe [\[1\]](https://youtu.be/U_u7nYokzSU).
- Entity portal dupe.
- Rail and carpet dupe.
- TileEntity chunk ban.
- Not accepting books longer than 50 pages.
- Do not accept an editing or book signing packet if the book is not in hand.
- StackOverflowError while loading chunk entities.
- Do not load chunks on adjacent chest check.
- Clientside entity desynchronization.
- Paper's collision disable for custom scoreboards.
- Oversized bounding box on dismount crash.
- Dispencer shulker box crash [\[1\]](https://youtu.be/zFrCb1RVyys?t=104).
- Reduce EntityTracker memory leakage.

[Unreleased]: https://github.com/ruViolence/Reaper/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/ruViolence/Reaper/releases/tag/v1.0.0