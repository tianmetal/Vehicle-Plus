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
native CreateVehicle(modelid, Float:x, Float:y, Float:z, Float:rotation, color1 = -1, color2 = -1, respawn_delay = -1, addsiren = 0, worldid = 0, interiorid = 0, bool:unoccupied_damage = false);
native GetVehicleInterior(vehicleid);
native GetVehicleColor(vehicleid, &color1, &color2);
native GetVehiclePaintjob(vehicleid);
native RemoveVehiclePaintjob(vehicleid);
native SetVehicleHorn(vehicleid, soundid);
native GetVehicleHorn(vehicleid);
native RestoreVehicleHorn(vehicleid);
native ToggleVehicleDamageUpdate(vehicleid, type, bool:toggle);
native IsVehicleDamageToggled(vehicleid, type);
native UpdateVehicleDamageStatusEx(vehicleid, type, update);
native GetVehicleDamageStatusEx(vehicleid, type);
native IsVehicleOccupied(vehicleid);
native GetVehicleDriverID(vehicleid);
native EditVehicle(playerid, vehicleid);
native IsValidVehicle(vehicleid);
native GetVehicleName(vehicleid, string[], len = sizeof(string));
native GetVehicleModelName(modelid, string[], len = sizeof(string));
native SetVehicleParams(vehicleid, type, set);
native GetVehicleParams(vehicleid, type);
native Float:GetVehicleSpeed(vehicleid, bool:kmh = true, Float:velx = 0.0, Float:vely = 0.0, Float:velz = 0.0);
native IsObjectAttachedToVehicle(objectid, vehicleid);
native GetVehicleSlotAttachedObject(vehicleid, slot);
native TeleportVehicle(vehicleid, Float:x, Float:y, Float:z, Float:rotation, worldid = -1, interiorid = -1);
native SetVehicleSpeedCap(vehicleid, Float:maxspeed);
native Float:GetVehicleSpeedCap(vehicleid);
native DisableVehicleSpeedCap(vehicleid);
native GetVehicleTopSpeed(vehicleid);
native GetVehicleModelTopSpeed(modelid);
native SetVehicleSpawnInfo(vehicleid, Float:x, Float:y, Float:z, Float:rotation, worldid, interiorid);
native GetVehicleSpawnInfo(vehicleid, &Float:x, &Float:y, &Float:z, &Float:rotation, &worldid, &interiorid);
native ToggleUnoccupiedVehicleDamage(vehicleid, bool:toggle);
native IsUnoccupiedDamageToggled(vehicleid);
native ToggleVehiclePetrolCapDestroy(vehicleid, bool:toggle);
native IsPetrolCapDestroyToggled(vehicleid);
native SetVehicleBomb(vehicleid, time = 1000);
native GetVehicleBomb(vehicleid);
native RemoveVehicleBomb(vehicleid);
native IsVehicleBombed(vehicleid);
native IsVehicleBombActivated(vehicleid);
native ToggleVehicleSticky(vehicleid, bool:toggle);
native IsVehicleSticky(vehicleid);
native CountAllVehicles();
native DestroyAllVehicles();

CALLBACKS:
public OnPlayerShotVehicle(playerid, vehicleid, weaponid, Float:amount, bodypart)
public OnPlayerEditVehicle(playerid, vehicleid, response, Float:fX, Float:fY, Float:fZ, Float:fRotZ)
public OnPlayerReachSpeedCapLimit(playerid, vehicleid, Float:speed)
public OnVehicleBombActivate(vehicleid)
public OnVehicleBombDeactivate(vehicleid)
public OnVehicleBombExplode(vehicleid)
public OnVehiclePosChange(vehicleid, Float:newx, Float:newy, Float:newz, Float:newrotation, Float:oldx, Float:oldy, Float:oldz, Float:oldrotation)
public OnVehicleVelocityChange(vehicleid, Float:newx, Float:newy, Float:newz, Float:oldx, Float:oldy, Float:oldz)
public OnVehicleHealthChange(vehicleid, Float:newhealth, Float:oldhealth)
