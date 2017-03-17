# minecraft-crashreport

---- Minecraft Crash Report ----
// Everything's going to plan. No, really, that was supposed to happen.

Time: 3/16/17 12:01 PM
Description: Rendering Block Entity

java.lang.IllegalStateException: Already tesselating!
	at net.minecraft.client.renderer.Tessellator.func_78371_b(Tessellator.java:374)
	at net.minecraft.client.renderer.Tessellator.func_78382_b(Tessellator.java:364)
	at crazypants.enderio.machine.capbank.render.FillGauge.doRender(FillGauge.java:78)
	at crazypants.enderio.machine.capbank.render.FillGauge.render(FillGauge.java:68)
	at crazypants.enderio.machine.capbank.render.CapBankRenderer.func_147500_a(CapBankRenderer.java:173)
	at net.minecraft.client.renderer.tileentity.TileEntityRendererDispatcher.func_147549_a(SourceFile:100)
	at mrtjp.relocation.ASMHacks$.renderTileEntityAt(hacks.scala:30)
	at mrtjp.relocation.ASMHacks.renderTileEntityAt(hacks.scala)
	at net.minecraft.client.renderer.tileentity.TileEntityRendererDispatcher.func_147544_a(SourceFile:92)
	at net.minecraft.client.renderer.RenderGlobal.func_147589_a(RenderGlobal.java:781)
	at net.minecraft.client.renderer.EntityRenderer.func_78471_a(EntityRenderer.java:1599)
	at net.minecraft.client.renderer.EntityRenderer.func_78480_b(EntityRenderer.java:1337)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1001)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:898)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:483)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at net.minecraft.client.renderer.Tessellator.func_78371_b(Tessellator.java:374)
	at net.minecraft.client.renderer.Tessellator.func_78382_b(Tessellator.java:364)
	at crazypants.enderio.machine.capbank.render.FillGauge.doRender(FillGauge.java:78)
	at crazypants.enderio.machine.capbank.render.FillGauge.render(FillGauge.java:68)
	at crazypants.enderio.machine.capbank.render.CapBankRenderer.func_147500_a(CapBankRenderer.java:173)

-- Block Entity Details --
Details:
	Name: blockCapBankTileEntity // crazypants.enderio.machine.capbank.TileCapBank
	Block type: ID #1797 (tile.blockCapBank // crazypants.enderio.machine.capbank.BlockCapBank)
	Block data value: 3 / 0x3 / 0b0011
	Block location: World: (1267,58,1217), Chunk: (at 3,3,1 in 79,76; contains blocks 1264,0,1216 to 1279,255,1231), Region: (2,2; contains chunks 64,64 to 95,95, blocks 1024,0,1024 to 1535,255,1535)
	Actual block type: ID #1797 (tile.blockCapBank // crazypants.enderio.machine.capbank.BlockCapBank)
	Actual block data value: 3 / 0x3 / 0b0011
Stacktrace:
	at net.minecraft.client.renderer.tileentity.TileEntityRendererDispatcher.func_147549_a(SourceFile:100)
	at mrtjp.relocation.ASMHacks$.renderTileEntityAt(hacks.scala:30)
	at mrtjp.relocation.ASMHacks.renderTileEntityAt(hacks.scala)
	at net.minecraft.client.renderer.tileentity.TileEntityRendererDispatcher.func_147544_a(SourceFile:92)
	at net.minecraft.client.renderer.RenderGlobal.func_147589_a(RenderGlobal.java:781)
	at net.minecraft.client.renderer.EntityRenderer.func_78471_a(EntityRenderer.java:1599)

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityClientPlayerMP['cathyb06423'/207, l='MpServer', x=1268.07, y=58.99, z=1215.01]]
	Chunk stats: MultiplayerChunkCache: 625, 634
	Level seed: 0
	Level generator: ID 05 - BIOMESOP, ver 0. Features enabled: false
	Level generator options: 
	Level spawn location: World: (980,64,880), Chunk: (at 4,4,0 in 61,55; contains blocks 976,0,880 to 991,255,895), Region: (1,1; contains chunks 32,32 to 63,63, blocks 512,0,512 to 1023,255,1023)
	Level time: 689209 game time, 313591 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: true), thunder time: 0 (now: false)
	Level game mode: Game mode: creative (ID 1). Hardcore: false. Cheats: false
	Forced entities: 126 total; [EntityPig['Pig'/268, l='MpServer', x=1190.19, y=63.00, z=1161.44], EntitySheep['Sheep'/269, l='MpServer', x=1197.91, y=63.00, z=1154.94], EntitySheep['Sheep'/270, l='MpServer', x=1191.53, y=63.00, z=1152.47], EntityPig['Pig'/272, l='MpServer', x=1192.03, y=67.00, z=1166.41], EntityPig['Pig'/273, l='MpServer', x=1187.50, y=66.00, z=1163.69], EntityPig['Pig'/275, l='MpServer', x=1193.31, y=64.00, z=1162.09], EntitySheep['Sheep'/276, l='MpServer', x=1193.44, y=67.00, z=1166.38], EntityPig['Pig'/277, l='MpServer', x=1197.25, y=70.00, z=1174.53], EntityPig['Pig'/278, l='MpServer', x=1189.09, y=70.00, z=1184.22], EntityPig['Pig'/279, l='MpServer', x=1197.06, y=71.00, z=1187.25], EntityPig['Pig'/280, l='MpServer', x=1198.81, y=68.00, z=1205.88], EntitySheep['Sheep'/281, l='MpServer', x=1194.31, y=69.00, z=1204.25], EntitySheep['Sheep'/282, l='MpServer', x=1197.38, y=69.00, z=1205.34], EntityPig['Pig'/283, l='MpServer', x=1195.44, y=69.00, z=1214.56], EntityPig['Pig'/284, l='MpServer', x=1189.13, y=66.00, z=1220.31], EntityPig['Pig'/285, l='MpServer', x=1192.91, y=70.00, z=1244.13], EntityPig['Pig'/290, l='MpServer', x=1213.88, y=69.00, z=1178.41], EntitySheep['Sheep'/291, l='MpServer', x=1204.19, y=69.00, z=1199.25], EntityPig['Pig'/292, l='MpServer', x=1211.34, y=70.00, z=1206.84], EntityPig['Pig'/293, l='MpServer', x=1212.50, y=71.00, z=1200.31], EntityPig['Pig'/294, l='MpServer', x=1207.97, y=70.00, z=1207.94], EntityPig['Pig'/295, l='MpServer', x=1205.66, y=68.00, z=1220.47], EntityPig['Pig'/296, l='MpServer', x=1210.13, y=69.00, z=1231.81], EntityPig['Pig'/297, l='MpServer', x=1201.19, y=66.00, z=1246.34], EntityPig['Pig'/298, l='MpServer', x=1215.91, y=71.00, z=1237.31], EntityPig['Pig'/299, l='MpServer', x=1198.47, y=67.85, z=1246.33], EntityPig['Pig'/300, l='MpServer', x=1211.50, y=64.00, z=1256.19], EntityPig['Pig'/301, l='MpServer', x=1212.50, y=67.96, z=1250.46], EntityPig['Pig'/310, l='MpServer', x=1223.53, y=64.00, z=1144.66], EntityPig['Pig'/311, l='MpServer', x=1223.22, y=68.00, z=1175.66], EntityPig['Pig'/312, l='MpServer', x=1230.75, y=71.00, z=1203.91], EntityPig['Pig'/313, l='MpServer', x=1220.63, y=73.00, z=1207.22], EntityChicken['Chicken'/314, l='MpServer', x=1230.47, y=67.00, z=1204.65], EntityPig['Pig'/315, l='MpServer', x=1218.84, y=71.00, z=1220.03], EntityPig['Pig'/316, l='MpServer', x=1223.78, y=71.00, z=1210.66], EntitySheep['Sheep'/317, l='MpServer', x=1213.97, y=71.00, z=1242.03], EntityPig['Pig'/318, l='MpServer', x=1229.31, y=80.00, z=1269.50], EntityPig['Pig'/320, l='MpServer', x=1235.19, y=67.00, z=1138.16], EntityPig['Pig'/321, l='MpServer', x=1240.72, y=68.00, z=1143.16], EntitySheep['Sheep'/322, l='MpServer', x=1231.84, y=67.00, z=1145.16], EntityChicken['Chicken'/323, l='MpServer', x=1236.53, y=70.00, z=1198.41], EntityPig['Pig'/324, l='MpServer', x=1238.47, y=66.00, z=1211.69], EntityPig['Pig'/325, l='MpServer', x=1233.97, y=67.00, z=1220.06], EntityPig['Pig'/326, l='MpServer', x=1247.97, y=74.00, z=1270.03], EntityChicken['Chicken'/327, l='MpServer', x=1240.66, y=75.00, z=1287.38], EntityChicken['Chicken'/328, l='MpServer', x=1240.59, y=78.00, z=1286.53], EntityPig['Pig'/332, l='MpServer', x=1253.16, y=68.00, z=1138.22], EntityPig['Pig'/333, l='MpServer', x=1254.34, y=68.00, z=1139.50], EntityPig['Pig'/334, l='MpServer', x=1251.81, y=69.00, z=1147.06], EntitySquid['Squid'/335, l='MpServer', x=1248.47, y=51.39, z=1198.65], EntityChicken['Chicken'/336, l='MpServer', x=1253.19, y=63.00, z=1194.16], EntityChicken['Chicken'/337, l='MpServer', x=1248.78, y=64.00, z=1196.53], EntityChicken['Chicken'/338, l='MpServer', x=1254.30, y=63.87, z=1195.89], EntityChicken['Chicken'/339, l='MpServer', x=1255.22, y=64.00, z=1196.88], EntityChicken['Chicken'/340, l='MpServer', x=1253.81, y=64.00, z=1197.97], EntityChicken['Chicken'/341, l='MpServer', x=1254.59, y=64.00, z=1198.56], EntityChicken['Chicken'/342, l='MpServer', x=1249.25, y=64.00, z=1197.41], EntityChicken['Chicken'/343, l='MpServer', x=1248.79, y=64.00, z=1200.12], EntityChicken['Chicken'/344, l='MpServer', x=1250.38, y=64.00, z=1196.03], EntityChicken['Chicken'/345, l='MpServer', x=1248.72, y=64.00, z=1195.13], EntityChicken['Chicken'/346, l='MpServer', x=1255.28, y=64.00, z=1198.84], EntityChicken['Chicken'/347, l='MpServer', x=1255.28, y=64.00, z=1198.53], EntityChicken['Chicken'/348, l='MpServer', x=1248.72, y=64.00, z=1196.94], EntityChicken['Chicken'/349, l='MpServer', x=1255.28, y=64.00, z=1197.47], EntityChicken['Chicken'/350, l='MpServer', x=1255.28, y=64.00, z=1195.47], EntityChicken['Chicken'/351, l='MpServer', x=1248.72, y=64.00, z=1195.81], EntityChicken['Chicken'/352, l='MpServer', x=1255.28, y=64.00, z=1195.13], EntityChicken['Chicken'/353, l='MpServer', x=1248.78, y=64.85, z=1199.58], EntityItem['item.item.feather'/354, l='MpServer', x=1250.56, y=64.13, z=1195.81], EntityChicken['Chicken'/355, l='MpServer', x=1249.33, y=63.00, z=1195.50], EntityChicken['Chicken'/356, l='MpServer', x=1248.78, y=64.00, z=1197.94], EntityChicken['Chicken'/357, l='MpServer', x=1248.78, y=64.00, z=1198.87], EntityItem['item.item.feather'/358, l='MpServer', x=1253.72, y=64.13, z=1197.66], EntityChicken['Chicken'/359, l='MpServer', x=1254.09, y=64.00, z=1197.19], EntityChicken['Chicken'/360, l='MpServer', x=1255.28, y=64.00, z=1199.25], EntityChicken['Chicken'/361, l='MpServer', x=1255.22, y=64.96, z=1200.71], EntityChicken['Chicken'/362, l='MpServer', x=1250.63, y=64.00, z=1196.63], EntityChicken['Chicken'/363, l='MpServer', x=1253.31, y=64.00, z=1199.56], EntityChicken['Chicken'/364, l='MpServer', x=1254.94, y=64.00, z=1196.34], EntityChicken['Chicken'/365, l='MpServer', x=1254.38, y=64.00, z=1196.49], EntityChicken['Chicken'/366, l='MpServer', x=1249.34, y=64.00, z=1198.97], EntityBat['Bat'/367, l='MpServer', x=1246.77, y=18.37, z=1201.64], EntityBat['Bat'/368, l='MpServer', x=1250.25, y=54.10, z=1203.41], EntitySquid['Squid'/369, l='MpServer', x=1250.47, y=51.00, z=1203.53], EntityItem['item.item.dyePowder.black'/370, l='MpServer', x=1258.88, y=53.88, z=1208.88], EntitySquid['Squid'/371, l='MpServer', x=1255.52, y=51.00, z=1202.51], EntitySquid['Squid'/372, l='MpServer', x=1254.69, y=51.00, z=1200.47], EntityChicken['Chicken'/373, l='MpServer', x=1248.72, y=64.00, z=1200.59], EntityChicken['Chicken'/374, l='MpServer', x=1255.28, y=64.00, z=1200.50], EntityChicken['Chicken'/375, l='MpServer', x=1254.59, y=64.00, z=1199.92], EntityChicken['Chicken'/376, l='MpServer', x=1249.31, y=64.00, z=1200.16], EntityChicken['Chicken'/377, l='MpServer', x=1254.69, y=64.00, z=1199.13], EntityChicken['Chicken'/378, l='MpServer', x=1255.22, y=64.00, z=1199.75], EntityChicken['Chicken'/379, l='MpServer', x=1254.47, y=64.00, z=1200.84], EntityChicken['Chicken'/386, l='MpServer', x=1269.28, y=65.00, z=1144.53], EntitySheep['Sheep'/387, l='MpServer', x=1276.63, y=65.00, z=1148.47], EntityPig['Pig'/388, l='MpServer', x=1277.28, y=68.00, z=1265.13], EntityPig['Pig'/389, l='MpServer', x=1277.53, y=68.00, z=1292.66], EntityPig['Pig'/391, l='MpServer', x=1288.75, y=64.00, z=1155.59], EntitySheep['Sheep'/392, l='MpServer', x=1293.16, y=64.00, z=1154.63], EntityPig['Pig'/393, l='MpServer', x=1296.97, y=64.00, z=1160.06], EntitySheep['Sheep'/394, l='MpServer', x=1295.88, y=64.00, z=1163.19], EntityPig['Pig'/395, l='MpServer', x=1293.31, y=69.00, z=1180.50], EntityPig['Pig'/396, l='MpServer', x=1281.16, y=68.00, z=1267.81], EntityBat['Bat'/397, l='MpServer', x=1309.63, y=16.10, z=1190.75], EntityBat['Bat'/398, l='MpServer', x=1307.25, y=16.10, z=1189.75], EntityItem['item.item.reeds'/399, l='MpServer', x=1302.13, y=65.13, z=1229.66], EntityPig['Pig'/400, l='MpServer', x=1300.28, y=69.00, z=1256.09], EntityBat['Bat'/401, l='MpServer', x=1303.00, y=49.00, z=1276.03], EntityBat['Bat'/402, l='MpServer', x=1297.53, y=49.00, z=1275.75], EntityBat['Bat'/407, l='MpServer', x=1322.69, y=27.10, z=1165.78], EntityBat['Bat'/408, l='MpServer', x=1321.31, y=33.00, z=1159.91], EntityPig['Pig'/409, l='MpServer', x=1316.16, y=63.00, z=1157.88], EntitySheep['Sheep'/410, l='MpServer', x=1324.81, y=63.00, z=1180.63], EntityPig['Pig'/411, l='MpServer', x=1328.19, y=63.00, z=1173.16], EntityPig['Pig'/412, l='MpServer', x=1315.41, y=63.00, z=1168.25], EntityPig['Pig'/413, l='MpServer', x=1313.91, y=73.00, z=1278.22], EntityCartChest['entity.MinecartChest.name'/425, l='MpServer', x=1338.50, y=30.50, z=1091.50], EntityChicken['Chicken'/429, l='MpServer', x=1330.44, y=62.03, z=1170.59], EntityPig['Pig'/430, l='MpServer', x=1338.50, y=84.00, z=1216.50], EntityBat['Bat'/431, l='MpServer', x=1331.56, y=46.00, z=1246.78], EntityPig['Pig'/446, l='MpServer', x=1345.53, y=62.00, z=1243.38], EntityBat['Bat'/447, l='MpServer', x=1346.31, y=32.00, z=1289.00], EntityItem['item.item.feather'/718, l='MpServer', x=1248.13, y=64.13, z=1197.56], EntityClientPlayerMP['cathyb06423'/207, l='MpServer', x=1268.07, y=58.99, z=1215.01], EntityCartChest['entity.MinecartChest.name'/482, l='MpServer', x=1397.50, y=37.50, z=1128.50]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:425)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2444)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:919)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:483)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_25, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 1517965960 bytes (1447 MB) / 3467640832 bytes (3307 MB) up to 8321499136 bytes (7936 MB)
	JVM Flags: 5 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx8G -Xms3G -Xmn768m -XX:ReservedCodeCacheSize=2048m
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 15, tallocated: 96
	FML: MCP v9.05 FML v7.10.99.99 Minecraft Forge 10.13.4.1614 Optifine OptiFine_1.7.10_HD_U_D6 110 mods loaded, 110 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCHIJAAAA	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) 
	UCHIJAAAA	FML{7.10.99.99} [Forge Mod Loader] (forge-1.7.10-10.13.4.1614-1.7.10.jar) 
	UCHIJAAAA	Forge{10.13.4.1614} [Minecraft Forge] (forge-1.7.10-10.13.4.1614-1.7.10.jar) 
	UCHIJAAAA	da3dsoulASMFix{0.1.0} [DA3DSOUL ASM Fixes] (minecraft.jar) 
	UCHIJAAAA	appliedenergistics2-core{rv3-beta-6} [Applied Energistics 2 Core] (minecraft.jar) 
	UCHIJAAAA	CodeChickenCore{1.0.7.47} [CodeChicken Core] (minecraft.jar) 
	UCHIJAAAA	NotEnoughItems{1.0.5.120} [Not Enough Items] (NotEnoughItems-1.7.10-1.0.5.120-universal.jar) 
	UCHIJAAAA	OpenModsCore{0.10} [OpenModsCore] (minecraft.jar) 
	UCHIJAAAA	<CoFH ASM>{000} [CoFH ASM] (minecraft.jar) 
	UCHIJAAAA	<DragonAPI ASM>{0} [DragonAPI ASM Data Initialization] (minecraft.jar) 
	UCHIJAAAA	mod_ThreadedLighting{1.7.10-1.0} [Threaded Lighting] (minecraft.jar) 
	UCHIJAAAA	gilded-games-util{1.7.10-1.2} [Gilded Games Utility] (gilded-games-util-1.7.10-1.9.jar) 
	UCHIJAAAA	bspkrsCore{6.15} [bspkrsCore] ([1.7.10]bspkrsCore-universal-6.15.jar) 
	UCHIJAAAA	Treecapitator{1.7.10} [Treecapitator] ([1.7.10]Treecapitator-universal-2.0.4.jar) 
	UCHIJAAAA	CoFHCore{1.7.10R3.1.3} [CoFH Core] (CoFHCore-[1.7.10]3.1.3-327.jar) 
	UCHIJAAAA	BuildCraft|Core{7.1.18} [BuildCraft] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	BuildCraft|Transport{7.1.18} [BC Transport] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	BuildCraft|Silicon{7.1.18} [BC Silicon] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	BuildCraft|Energy{7.1.18} [BC Energy] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	BuildCraft|Factory{7.1.18} [BC Factory] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	BuildCraft|Builders{7.1.18} [BC Builders] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	Baubles{1.0.1.10} [Baubles] (Baubles-1.7.10-1.0.1.10.jar) 
	UCHIJAAAA	ThermalFoundation{1.7.10R1.2.5} [Thermal Foundation] (ThermalFoundation-[1.7.10]1.2.5-115.jar) 
	UCHIJAAAA	ThermalExpansion{1.7.10R4.1.4} [Thermal Expansion] (ThermalExpansion-[1.7.10]4.1.4-247.jar) 
	UCHIJAAAA	Additional-Buildcraft-Objects{MC1.7.10-BC7.1release4.0.9} [Additional Buildcraft Objects] (ABO-MC1.7.10-BC7.1release4.0.9.jar) 
	UCHIJAAAA	appliedenergistics2{rv3-beta-6} [Applied Energistics 2] (appliedenergistics2-rv3-beta-6.jar) 
	UCHIJAAAA	bdlib{1.9.4.109} [BD Lib] (bdlib-1.9.4.109-mc1.7.10.jar) 
	UCHIJAAAA	ae2stuff{0.5.0.56} [AE2 Stuff] (ae2stuff-0.5.0.56-mc1.7.10.jar) 
	UCHIJAAAA	aether{1.7.10-1.6} [Aether II] (aether-1.7.10-1.6.jar) 
	UCHIJAAAA	AgriCraft{1.7.10-1.5.0} [AgriCraft] (AgriCraft-1.7.10-1.5.0.jar) 
	UCHIJAAAA	bis{3.1.6} [Back in Slime Mod] (Back In Slime-1.7.10-3.1.6.jar) 
	UCHIJAAAA	bagginses{2.1.1} [Bagginses] (Bagginses-2.1.1.jar) 
	UCHIJAAAA	baublelicious{1.7.10-1.2.2-final} [Baublelicious] (baublelicious-1.7.10-1.2.2-final.jar) 
	UCHIJAAAA	BiblioCraft{1.11.5} [BiblioCraft] (BiblioCraft[v1.11.5][MC1.7.10].jar) 
	UCHIJAAAA	Mantle{1.7.10-0.3.2.jenkins191} [Mantle] (Mantle-1.7.10-0.3.2b.jar) 
	UCHIJAAAA	Natura{2.2.0} [Natura] (natura-1.7.10-2.2.0.1.jar) 
	UCHIJAAAA	BiomesOPlenty{2.1.0} [Biomes O' Plenty] (BiomesOPlenty-1.7.10-2.1.0.2027-universal.jar) 
	UCHIJAAAA	BiblioWoodsBoP{1.9} [BiblioWoods Biomes O'Plenty Edition] (BiblioWoods[BiomesOPlenty][v1.9].jar) 
	UCHIJAAAA	ExtrabiomesXL{3.16.4} [ExtrabiomesXL] (extrabiomesxl_1.7.10-3.16.4.jar) 
	UCHIJAAAA	BiblioWoodsEBXL{1.4} [BiblioWoods ExtraBiomesXL Edition] (BiblioWoods[ExtraBiomesXL][v1.4].jar) 
	UCHIJAAAA	IC2{2.2.823-experimental} [IndustrialCraft 2] (industrialcraft-2-2.2.823-experimental.jar) 
	UCHIJAAAA	Forestry{4.2.16.64} [Forestry for Minecraft] (forestry_1.7.10-4.2.16.64.jar) 
	UCHIJAAAA	BiblioWoodsForestry{1.7} [BiblioWoods Forestry Edition] (BiblioWoods[Forestry][v1.7].jar) 
	UCHIJAAAA	BiblioWoodsNatura{1.5} [BiblioWoods Natura Edition] (BiblioWoods[Natura][v1.5].jar) 
	UCHIJAAAA	BigReactors{0.4.3A} [Big Reactors] (BigReactors-0.4.3A.jar) 
	UCHIJAAAA	Botania{r1.8-249} [Botania] (Botania r1.8-249.jar) 
	UCHIJAAAA	BuildCraft|Robotics{7.1.18} [BC Robotics] (buildcraft-7.1.18.jar) 
	UCHIJAAAA	BuildCraft|Compat{7.1.5} [BuildCraft Compat] (buildcraft-compat-7.1.5.jar) 
	UCHIJAAAA	Railcraft{9.12.2.0} [Railcraft] (Railcraft_1.7.10-9.12.2.0.jar) 
	UCHIJAAAA	ForgeMultipart{1.2.0.345} [Forge Multipart] (ForgeMultipart-1.7.10-1.2.0.345-universal.jar) 
	UCHIJAAAA	chisel{2.9.5.11} [Chisel] (Chisel-2.9.5.11.jar) 
	UCHIJAAAA	Mystcraft{0.12.3.03} [Mystcraft] (mystcraft-1.7.10-0.12.3.03.jar) 
	UCHIJAAAA	MrTJPCoreMod{1.1.0.33} [MrTJPCore] (MrTJPCore-1.7.10-1.1.0.33-universal.jar) 
	UCHIJAAAA	ProjRed|Core{4.7.0pre12.95} [ProjectRed Core] (ProjectRed-1.7.10-4.7.0pre12.95-Base.jar) 
	UCHIJAAAA	ExtraUtilities{1.2.12} [Extra Utilities] (extrautilities-1.2.12.jar) 
	UCHIJAAAA	ImmersiveEngineering{0.7.7} [Immersive Engineering] (ImmersiveEngineering-0.7.7.jar) 
	UCHIJAAAA	tc{4.3.1_007} [Traincraft] (Traincraft-4.3.1_007.jar) 
	UCHIJAAAA	Waila{1.5.10} [Waila] (Waila-1.5.10_1.7.10.jar) 
	UCHIJAAAA	TConstruct{1.7.10-1.8.8.build988} [Tinkers' Construct] (TConstruct-1.7.10-1.8.8.jar) 
	UCHIJAAAA	DragonAPI{1.0} [DragonAPI] (DragonAPI 1.7.10 V16d.jar) 
	UCHIJAAAA	endercore{1.7.10-0.2.0.36_beta} [EnderCore] (EnderCore-1.7.10-0.2.0.36_beta.jar) 
	UCHIJAAAA	EnderIO{1.7.10-2.3.0.429_beta} [Ender IO] (EnderIO-1.7.10-2.3.0.429_beta.jar) 
	UCHIJAAAA	enderioaddons{0.10.11} [Ender IO Addons] (EnderIOAddons-1.7.10-2.3.0.427_beta-0.10.11.54_beta.jar) 
	UCHIJAAAA	EnderStorage{1.4.7.37} [EnderStorage] (EnderStorage-1.7.10-1.4.7.37-universal.jar) 
	UCHIJAAAA	extracells{2.3.14} [Extra Cells 2] (ExtraCells-1.7.10-2.3.14b197.jar) 
	UCHIJAAAA	IC2NuclearControl{2.4.2a} [Nuclear Control 2] (IC2NuclearControl-2.4.2a.jar) 
	UCHIJAAAA	immersiveintegration{0.6.8} [Immersive Integration] (immersiveintegration-0.6.8.jar) 
	UCHIJAAAA	inventorytweaks{1.59-dev-152-cf6e263} [Inventory Tweaks] (InventoryTweaks-1.59-dev-152.jar) 
	UCHIJAAAA	journeymap{5.1.4p1} [JourneyMap] (journeymap-1.7.10-5.1.4p1-unlimited.jar) 
	UCHIJAAAA	LogisticsPipes{0.9.3.128} [Logistics Pipes] (logisticspipes-0.9.3.128.jar) 
	UCHIJAAAA	malisiscore{1.7.10-0.14.3} [MalisisCore] (malisiscore-1.7.10-0.14.3.jar) 
	UCHIJAAAA	malisisdoors{1.7.10-1.13.2} [Malisis' Doors] (malisisdoors-1.7.10-1.13.2.jar) 
	UCHIJAAAA	NEIAddons{1.12.14.40} [NEI Addons] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|Developer{1.12.14.40} [NEI Addons: Developer Tools] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|AppEng{1.12.14.40} [NEI Addons: Applied Energistics 2] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|Botany{1.12.14.40} [NEI Addons: Botany] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|Forestry{1.12.14.40} [NEI Addons: Forestry] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|CraftingTables{1.12.14.40} [NEI Addons: Crafting Tables] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|ExNihilo{1.12.14.40} [NEI Addons: Ex Nihilo] (neiaddons-1.12.14.40-mc1.7.10.jar) 
	UCHIJAAAA	neiintegration{1.1.2} [NEI Integration] (NEIIntegration-MC1.7.10-1.1.2.jar) 
	UCHIJAAAA	OpenMods{0.10} [OpenMods] (OpenModsLib-1.7.10-0.10.jar) 
	UCHIJAAAA	OpenBlocks{1.6} [OpenBlocks] (OpenBlocks-1.7.10-1.6.jar) 
	UCHIJAAAA	SonarCore{1.1.3} [SonarCore] (SonarCore-1.7.10-1.1.3.jar) 
	UCHIJAAAA	PracticalLogistics{0.2.4} [Practical Logistics] (Practical-Logistics-1.7.10-0.2.4.jar) 
	UCHIJAAAA	pressure{1.3.0.130} [Pressure Pipes] (pressure-1.3.0.130-mc1.7.10.jar) 
	UCHIJAAAA	ProjRed|Transmission{4.7.0pre12.95} [ProjectRed Transmission] (ProjectRed-1.7.10-4.7.0pre12.95-Integration.jar) 
	UCHIJAAAA	ProjRed|Transportation{4.7.0pre12.95} [ProjectRed Transportation] (ProjectRed-1.7.10-4.7.0pre12.95-Mechanical.jar) 
	UCHIJAAAA	ProjRed|Exploration{4.7.0pre12.95} [ProjectRed Exploration] (ProjectRed-1.7.10-4.7.0pre12.95-World.jar) 
	UCHIJAAAA	ProjRed|Compatibility{4.7.0pre12.95} [ProjectRed Compatibility] (ProjectRed-1.7.10-4.7.0pre12.95-Compat.jar) 
	UCHIJAAAA	ProjRed|Integration{4.7.0pre12.95} [ProjectRed Integration] (ProjectRed-1.7.10-4.7.0pre12.95-Integration.jar) 
	UCHIJAAAA	ProjRed|Fabrication{4.7.0pre12.95} [ProjectRed Fabrication] (ProjectRed-1.7.10-4.7.0pre12.95-Fabrication.jar) 
	UCHIJAAAA	ProjRed|Illumination{4.7.0pre12.95} [ProjectRed Illumination] (ProjectRed-1.7.10-4.7.0pre12.95-Lighting.jar) 
	UCHIJAAAA	ProjRed|Expansion{4.7.0pre12.95} [ProjectRed Expansion] (ProjectRed-1.7.10-4.7.0pre12.95-Mechanical.jar) 
	UCHIJAAAA	RotaryCraft{1.0} [RotaryCraft] (RotaryCraft 1.7.10 V16d.jar) 
	UCHIJAAAA	ReactorCraft{1.0} [ReactorCraft] (ReactorCraft 1.7.10 V16d.jar) 
	UCHIJAAAA	ThermalDynamics{1.7.10R1.2.0} [Thermal Dynamics] (ThermalDynamics-[1.7.10]1.2.0-171.jar) 
	UCHIJAAAA	ThermalSmeltery{1.0} [Thermal Smeltery] (ThermalSmeltery-1.3.1.4.jar) 
	UCHIJAAAA	TiConAutoToolStation{1.1.2} [Tinkers Construct Auto Tool Station] (TiConAutoToolStation-1.7.10-1.1.2.jar) 
	UCHIJAAAA	tinker_io{release 1.5.0} [Tinker I/O] (tinker_io-1.7.10-release 1.5.0.jar) 
	UCHIJAAAA	UltraTech{1.7.10-0.9.6.1} [UltraTech] (Ultratech-1.7.10-0.9.6.1.jar) 
	UCHIJAAAA	WailaHarvestability{1.1.6} [Waila Harvestability] (WailaHarvestability-mc1.7.10-1.1.6.jar) 
	UCHIJAAAA	wailaplugins{MC1.7.10-0.2.0-25} [WAILA Plugins] (WAILAPlugins-MC1.7.10-0.2.0-25.jar) 
	UCHIJAAAA	wawla{1.3.1} [What Are We Looking At] (Wawla-1.0.5.120.jar) 
	UCHIJAAAA	worldedit{6.1.1} [WorldEdit] (worldedit-forge-mc1.7.10-6.1.1-dist.jar) 
	UCHIJAAAA	McMultipart{1.2.0.345} [Minecraft Multipart Plugin] (ForgeMultipart-1.7.10-1.2.0.345-universal.jar) 
	UCHIJAAAA	ForgeRelocation{0.0.1.4} [ForgeRelocation] (ForgeRelocation-1.7.10-0.0.1.4-universal.jar) 
	UCHIJAAAA	MCFrames{1.0} [MCFrames] (ForgeRelocation-1.7.10-0.0.1.4-universal.jar) 
	UCHIJAAAA	RelocationFMP{0.0.1.2} [RelocationFMP] (ForgeRelocationFMP-1.7.10-0.0.1.2-universal.jar) 
	UCHIJAAAA	aobd{2.9.2} [Another One Bites The Dust] (AOBD-2.9.2.jar) 
	UCHIJAAAA	ForgeMicroblock{1.2.0.345} [Forge Microblocks] (ForgeMultipart-1.7.10-1.2.0.345-universal.jar) 
	GL info: ' Vendor: 'NVIDIA Corporation' Version: '4.5.0 NVIDIA 378.78' Renderer: 'GeForce GTX 970/PCIe/SSE2'
	OpenModsLib class transformers: [stencil_patches:FINISHED],[movement_callback:FINISHED],[player_damage_hook:FINISHED],[map_gen_fix:FINISHED],[gl_capabilities_hook:FINISHED],[player_render_hook:FINISHED]
	Class transformer null safety: all safe
	CoFHCore: -[1.7.10]3.1.3-327
	ThermalFoundation: -[1.7.10]1.2.5-115
	ThermalExpansion: -[1.7.10]4.1.4-247
	AE2 Version: beta rv3-beta-6 for Forge 10.13.4.1448
	Mantle Environment: DO NOT REPORT THIS CRASH! Unsupported mods in environment: optifine
	TConstruct Environment: Environment healthy.
	ThermalDynamics: -[1.7.10]1.2.0-171
	List of loaded APIs: 
		* AgriCraftAPI (1.0) from AgriCraft-1.7.10-1.5.0.jar
		* appliedenergistics2|API (rv2) from DragonAPI 1.7.10 V16d.jar
		* Baubles|API (1.0.1.10) from Baubles-1.7.10-1.0.1.10.jar
		* BiomesOPlentyAPI (1.0.0) from BiomesOPlenty-1.7.10-2.1.0.2027-universal.jar
		* BotaniaAPI (76) from Botania r1.8-249.jar
		* BuildCraftAPI|blocks (1.0) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|blueprints (1.5) from buildcraft-7.1.18.jar
		* BuildCraftAPI|boards (2.0) from buildcraft-7.1.18.jar
		* BuildCraftAPI|core (1.0) from Ultratech-1.7.10-0.9.6.1.jar
		* BuildCraftAPI|crops (1.1) from buildcraft-7.1.18.jar
		* BuildCraftAPI|events (2.0) from buildcraft-7.1.18.jar
		* BuildCraftAPI|facades (1.1) from buildcraft-7.1.18.jar
		* BuildCraftAPI|filler (4.0) from buildcraft-7.1.18.jar
		* BuildCraftAPI|fuels (1.0) from Ultratech-1.7.10-0.9.6.1.jar
		* BuildCraftAPI|gates (4.1) from buildcraft-7.1.18.jar
		* BuildCraftAPI|items (1.1) from buildcraft-7.1.18.jar
		* BuildCraftAPI|library (2.0) from buildcraft-7.1.18.jar
		* BuildCraftAPI|lists (1.0) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|mj (1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* BuildCraftAPI|power (1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* BuildCraftAPI|recipes (3.0) from buildcraft-7.1.18.jar
		* BuildCraftAPI|robotics (3.0) from buildcraft-7.1.18.jar
		* BuildCraftAPI|statements (1.1) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|tablet (1.0) from Railcraft_1.7.10-9.12.2.0.jar
		* BuildCraftAPI|tiles (1.2) from buildcraft-7.1.18.jar
		* BuildCraftAPI|tools (1.0) from extrautilities-1.2.12.jar
		* BuildCraftAPI|transport (2.0) from Ultratech-1.7.10-0.9.6.1.jar
		* ChiselAPI (0.1.1) from Chisel-2.9.5.11.jar
		* ChiselAPI|Carving (0.1.1) from Chisel-2.9.5.11.jar
		* ChiselAPI|Rendering (0.1.1) from Chisel-2.9.5.11.jar
		* CoFHAPI (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHAPI|block (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHAPI|core (1.7.10R1.1.0) from SonarCore-1.7.10-1.1.3.jar
		* CoFHAPI|energy (1.7.10R1.0.1) from Ultratech-1.7.10-0.9.6.1.jar
		* CoFHAPI|fluid (1.7.10R1.1.0) from SonarCore-1.7.10-1.1.3.jar
		* CoFHAPI|inventory (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHAPI|item (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHAPI|modhelpers (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHAPI|tileentity (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHAPI|transport (1.7.10R1.0.13) from EnderCore-1.7.10-0.2.0.36_beta.jar
		* CoFHAPI|world (1.7.10R1.3.1) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|audio (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|gui (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|gui|container (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|gui|element (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|gui|element|listbox (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|gui|slot (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|inventory (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|render (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|render|particle (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|util (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|util|helpers (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|util|position (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|world (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* CoFHLib|world|feature (1.7.10R1.1.2) from CoFHCore-[1.7.10]3.1.3-327.jar
		* EnderIOAPI (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* EnderIOAPI|Redstone (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* EnderIOAPI|Teleport (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* EnderIOAPI|Tools (0.0.2) from EnderIO-1.7.10-2.3.0.429_beta.jar
		* ForestryAPI|apiculture (4.8.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|arboriculture (4.2.1) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|circuits (3.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|core (5.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|farming (2.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|food (1.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|fuels (2.0.1) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|genetics (4.7.1) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|hives (4.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|lepidopterology (1.3.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|mail (3.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|multiblock (3.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|recipes (5.4.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|storage (3.0.0) from forestry_1.7.10-4.2.16.64.jar
		* ForestryAPI|world (2.1.0) from forestry_1.7.10-4.2.16.64.jar
		* ForgeRelocation|API (0.0.1.4) from ForgeRelocation-1.7.10-0.0.1.4-universal.jar
		* IC2API (1.0) from SonarCore-1.7.10-1.1.3.jar
		* ImmersiveEngineering|API (1.0) from ImmersiveEngineering-0.7.7.jar
		* minechemAPI (1.7.10R1) from DragonAPI 1.7.10 V16d.jar
		* Mystcraft|API (0.1) from mystcraft-1.7.10-0.12.3.03.jar
		* NuclearControlAPI (v1.0.5) from IC2NuclearControl-2.4.2a.jar
		* OpenBlocks|API (1.1) from OpenBlocks-1.7.10-1.6.jar
		* PracticalLogisticsAPI (1.4) from Practical-Logistics-1.7.10-0.2.4.jar
		* pressureAPI (1.3.0.130) from pressure-1.3.0.130-mc1.7.10.jar
		* RailcraftAPI|bore (1.0.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|carts (1.6.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|core (1.5.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|crafting (1.0.0) from ImmersiveEngineering-0.7.7.jar
		* RailcraftAPI|electricity (2.0.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|events (1.0.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|fuel (1.0.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|helpers (1.1.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|items (1.0.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|locomotive (1.1.0) from Railcraft_1.7.10-9.12.2.0.jar
		* RailcraftAPI|signals (2.3.0) from Traincraft-4.3.1_007.jar
		* RailcraftAPI|tracks (2.3.0) from Railcraft_1.7.10-9.12.2.0.jar
		* Thaumcraft|API (4.2.2.0) from Railcraft_1.7.10-9.12.2.0.jar
		* UltratechAPI (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Power (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Power|Interfaces (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Power|Multipart (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Power|PreFab (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Reactor (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Recipes (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Refinery (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* UltratechAPI|Util (1.1.1) from Ultratech-1.7.10-0.9.6.1.jar
		* WailaAPI (1.2) from Waila-1.5.10_1.7.10.jar
	Chisel: Errors like "[FML]: Unable to lookup ..." are NOT the cause of this crash. You can safely ignore these errors. And update forge while you're at it.
	EnderIO: Found the following problem(s) with your installation:
                  * Optifine is installed. This is NOT supported.
                  * An unsupportted old RF API is installed (1.7.10R1.0.1 from Ultratech-1.7.10-0.9.6.1.jar).
                    Ender IO needs at least 1.7.10R1.0.2 and will NOT work with older versions.
                 This may have caused the error. Try reproducing the crash WITHOUT this/these mod(s) before reporting it.
	Stencil buffer state: Function set: GL30, pool: forge, bits: 8
	Forestry : Warning: You have mods that change the behavior of Minecraft, ForgeModLoader, and/or Minecraft Forge to your client: 
Optifine
These may have caused this error, and may not be supported. Try reproducing the crash WITHOUT these mods, and report it then.
	AE2 Integration: IC2:ON, RotaryCraft:ON, RC:ON, BuildCraftCore:ON, BuildCraftTransport:ON, BuildCraftBuilder:ON, RF:ON, RFItem:ON, MFR:OFF, DSU:ON, FZ:OFF, FMP:ON, RB:OFF, CLApi:OFF, Waila:ON, InvTweaks:ON, NEI:ON, CraftGuide:OFF, Mekanism:OFF, ImmibisMicroblocks:OFF, BetterStorage:OFF, OpenComputers:OFF, PneumaticCraft:OFF
	Launched Version: 1.7.10-Forge10.13.4.1614-1.7.10
	LWJGL: 2.9.1
	OpenGL: GeForce GTX 970/PCIe/SSE2 GL version 4.5.0 NVIDIA 378.78, NVIDIA Corporation
	GL Caps: Using GL 1.3 multitexturing.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Anisotropic filtering is supported and maximum anisotropy is 16.
Shaders are available because OpenGL 2.1 is supported.

	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: [OCDpack1.7.zip, Fanver_Modded_Universal (1).zip]
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Anisotropic Filtering: Off (1)
	OptiFine Version: OptiFine_1.7.10_HD_U_D6
	Render Distance Chunks: 12
	Mipmaps: 4
	Anisotropic Filtering: 1
	Antialiasing: 0
	Multitexture: false
	OpenGlVersion: 4.5.0 NVIDIA 378.78
	OpenGlRenderer: GeForce GTX 970/PCIe/SSE2
	OpenGlVendor: NVIDIA Corporation
	CpuCount: 8
