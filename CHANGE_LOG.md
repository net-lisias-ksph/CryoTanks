# CryoTanks :: Change Log

* 2019-1106: 1.4.0 (Nertea) for KSP 1.8.
	+ KSP 1.8.x
	+ Updated B9PartSwitch to 2.12.1
	+ Updated DynamicBatteryStorage to 2.1.0
	+ Updated ModuleManger to 4.1.0
	+ Updated CRP to 1.3.0
	+ Updated .NET version to 4.5
	+ Updated some MM patch specifiers
* 2019-0911: 1.3.0 (Nertea) for KSP 1.6.1
	+ Updated B9PartSwitch to 2.10.0
	+ Updated DynamicBatteryStorage to 2.0.6
	+ Fixed LCH4/Ox tank mass ratio issue
	+ Improved end-user documentation for features that are not enabled by default
	+ A few under the hood bug fixes/edge cases have been addressed
	+ Several under the hood efficiency improvements
	+ Some minor UI tweaks and fixes
	+ It is now possible to specify different cooling costs per fuel type in configs
* 2019-0809: 1.2.3 (Nertea) for KSP 1.6.1
	+ Updated DynamicBatteryStorage to 2.0.5
	+ Added Chinese translation (6DYZBX)
	+ Added LCH4 ISRU support (enabled with the same conditions as LCH4 tankage)
* 2019-0731: 1.2.2 (Nertea) for KSP 1.6.1
	+ Updated B9PartSwitch to 2.9.0
	+ Updated DynamicBatteryStorage to 2.0.4
	+ Made use of B9PartSwitch 2.9.0 features in several parts (UI colours, tooltips)
* 2019-0729: 1.2.1 (Nertea) for KSP 1.6.1
	+ Updated DynamicBatteryStorage to 2.0.3
	+ Moved each ZBO tank to be one tech node above corresponding regular tank (Wyzard256's suggestion)
* 2019-0726: 1.2.0 (Nertea) for KSP 1.6.1
	+ Updated B9PartSwitch to 2.8.1
	+ Updated DynamicBatteryStorage to 2.0.2
		- Added support for GenericFieldDataHandler     * Fixed FissionFlowRadiator adding heat to the simulation instead of removing it
		- Fixed two instances of null reference exceptions when switching vessels/scenes
	+ Fixed a localization typo
	+ Tuned VAB UI part tooltip fields for boiloff module
	+ Reworked textures of foil tanks to match Restock and Near Future Construction
	+ Normalized grey to be similar to all my other mods
	+ Recompressed all textures with better compression algorithm
	+ Added optional simplistic draft Liquid Methane support
		- Slightly cryogenic (1/10th the boiloff rate of Liquid Hydrogen)
		- Similar mass ratio to Liquid Fuel (9)
		- Higher cost ratio compared to Liquid Fuel (0.12 vs 0.1)
		- Enabled by declaring any MM patch with :FOR[CryoTanksMethalox] or including a folder in GameData called CryoTanksMethalox
* 2019-0709: 1.1.4 (Nertea) for KSP 1.6.1
	+ Updated B9PartSwitch to 2.8.0
	+ Updated DynamicBatteryStorage to 2.0.0
		- Complete rebuild
		- Mod now acts as a general power and thermal design tool as well as its previous functions
		- Added toolbar icon to open a Vessel Systems Management window
		- Vessel Systems Management Window
			- Allows player to view relevant Thermal and Electrical summary of the current vessel in VAB or flight
			- Electrical summary:
				- Shows whole-vessel power flows, separated into consumption and generation
				- VAB panel has a tool to simulate distance effects on solar panel efficiency
				- Estimates time to drain or time to charge batteries
				- Can drill down to part categories (eg. Solar Panels, Harvesters, etc)
				- Can drill down to individual parts
				- Handles these module types
					- Stock: ModuleDeployableSolarPanel, ModuleGenerator, ModuleResourceConverter, ModuleActiveRadiator, ModuleResourceHarvester, ModuleCommand, ModuleLight, ModuleDataTransmitter, ModuleEnginesFX, ModuleAlternator
					- NF Suite: ModuleCurvedSolarPanel, FissionGenerator, ModuleRadioisotopeGenerator, ModuleCryoTank, ModuleAntimatterTank, ModuleChargeableEngine, ModuleDeployableCentrifuge, DischargeCapacitor (partial)
					- RealBattery: RealBattery
					- Other: KopernicusSolarPanel
			- Thermal mode:
				- Shows whole-vessel core heat flows, separated into draw and generation
				- Can drill down to part categories (eg. Solar Panels, Harvesters, etc)
				- Can drill down to individual parts
				- NOTE: does not handle non-core heat(eg re-entry, engines, solar)
				- NOTE: does not make a distinction between adjacent-only radiators and full-vessel radiators
				- Handles relevant module types
					- Stock: ModuleCoreHeat (Passive heat only eg RTG), ModuleResourceConverter, ModuleActiveRadiator, ModuleResourceHarvester
					- NF Suite: FissionReactor, ModuleFusionCore
		- Customize settings with DynamicBatteryStorageSettings.cfg
	+ Changed LH2/O tank switcher patch to not activate cooling by default as such tanks are on average intended to be uncooled (thanks Zorg)
* 2019-0529: 1.1.3 (Nertea) for KSP 1.6.1
	+ Updated B9PartSwitch to 2.7.1
	+ Added updates to Russian translation from Sool3
	+ Improvements to LH2 switching patch which improves compatibility with mods that supply LH2/O tanks natively
* 2019-0415: 1.1.2 (Nertea) for KSP 1.6.1
	+ 1.7.x compatible
	+ Added French translation (thanks Aodh4n)
	+ Updated ModuleManger to 4.0.2
	+ Updated DynamicBatteryStorage to 1.4.1
	+ Updated B9PartSwitch to 2.7.0
	+ Fixed description of variants for compact 5m tank (thanks HSJasperism)
* 2019-0121: 1.1.1 (Nertea) for KSP 1.6.1
	+ No changelog provided
* 2019-0117: 1.1.0 (Nertea) for KSP 1.6.1
	+ No changelog provided
