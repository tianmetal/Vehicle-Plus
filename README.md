Vehicles Plus Include (vehicleplus.inc)
* Add new features to your vehicles system and have the missing or actually the correct word is needed vehicle functions
* Gives you advantage over ordinary vehicle manager includes, this is compatiable with other scripts (using property function)
* Now EditVehicle avalaible with this include

Author: (creator)
* Gammix

Contributors:
* Admigo - a_OPSVP include (offsets of vehicle bodyparts)
* Emmet_ - random car colors and top speed array

(c) Copyright 2015
* This file is provided as is (no warranties).

FUNCTIONS:
* CreateVehicle(modelid, Float:x, Float:y, Float:z, Float:rotation, color1 = -1, color2 = -1, respawn_delay = -1, addsiren = 0, worldid = 0, interiorid = 0, bool:unoccupied_damage = false);

* GetVehicleInterior(vehicleid);
* GetVehicleColor(vehicleid, &color1, &color2);
* GetVehiclePaintjob(vehicleid);
* RemoveVehiclePaintjob(vehicleid);
* SetVehicleHorn(vehicleid, soundid);
* GetVehicleHorn(vehicleid);
* RestoreVehicleHorn(vehicleid);
* ToggleVehicleDamageUpdate(vehicleid, type, bool:toggle);
* IsVehicleDamageToggled(vehicleid, type);
* UpdateVehicleDamageStatusEx(vehicleid, type, update);
* GetVehicleDamageStatusEx(vehicleid, type);
* IsVehicleOccupied(vehicleid);
* GetVehicleDriverID(vehicleid);
* EditVehicle(playerid, vehicleid);
* IsValidVehicle(vehicleid);
* GetVehicleName(vehicleid, string[], len = sizeof(string));
* GetVehicleModelName(modelid, string[], len = sizeof(string));
* SetVehicleParams(vehicleid, type, set);
* GetVehicleParams(vehicleid, type);
* Float:GetVehicleSpeed(vehicleid, bool:kmh = true, Float:velx = 0.0, Float:vely = 0.0, Float:velz = 0.0);
* IsObjectAttachedToVehicle(objectid, vehicleid);
* GetVehicleSlotAttachedObject(vehicleid, slot);
* TeleportVehicle(vehicleid, Float:x, Float:y, Float:z, Float:rotation, worldid = -1, interiorid = -1);
* SetVehicleSpeedCap(vehicleid, Float:maxspeed);
* Float:GetVehicleSpeedCap(vehicleid);
* DisableVehicleSpeedCap(vehicleid);
* GetVehicleTopSpeed(vehicleid);
* GetVehicleModelTopSpeed(modelid);
* SetVehicleSpawnInfo(vehicleid, Float:x, Float:y, Float:z, Float:rotation, worldid, interiorid);
* GetVehicleSpawnInfo(vehicleid, &Float:x, &Float:y, &Float:z, &Float:rotation, &worldid, &interiorid);
* ToggleUnoccupiedVehicleDamage(vehicleid, bool:toggle);
* IsUnoccupiedDamageToggled(vehicleid);
* ToggleVehiclePetrolCapDestroy(vehicleid, bool:toggle);
* IsPetrolCapDestroyToggled(vehicleid);
* SetVehicleBomb(vehicleid, time = 1000);
* GetVehicleBomb(vehicleid);
* RemoveVehicleBomb(vehicleid);
* IsVehicleBombed(vehicleid);
* IsVehicleBombActivated(vehicleid);
* ToggleVehicleSticky(vehicleid, bool:toggle);
* IsVehicleSticky(vehicleid);
* CountAllVehicles();
* DestroyAllVehicles();

CALLBACKS:
* public OnPlayerShotVehicle(playerid, vehicleid, weaponid, Float:amount, bodypart)
* public OnPlayerEditVehicle(playerid, vehicleid, response, Float:fX, Float:fY, Float:fZ, Float:fRotZ)
* public OnPlayerReachSpeedCapLimit(playerid, vehicleid, Float:speed)
* public OnVehicleBombActivate(vehicleid)
* public OnVehicleBombDeactivate(vehicleid)
* public OnVehicleBombExplode(vehicleid)
* public OnVehiclePosChange(vehicleid, Float:newx, Float:newy, Float:newz, Float:newrotation, Float:oldx, Float:oldy, Float:oldz, Float:oldrotation)
* public OnVehicleVelocityChange(vehicleid, Float:newx, Float:newy, Float:newz, Float:oldx, Float:oldy, Float:oldz)
* public OnVehicleHealthChange(vehicleid, Float:newhealth, Float:oldhealth)
