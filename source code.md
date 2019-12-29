options:
	name: AntiBuild
	version: 1.0
	
#		Made by Ecolipsy 1.0
#		Permissions: antibuild.break and antibuild.place and antibuild.drop
#		Commands: None

on block break:
	if player hasn't permission "antibuild.break":
		cancel event
		send "&4&lAntiBuild &6&l>> &cYou do not have permission to break blocks." to player

on block place:
	if player hasn't permission "antibuild.place":
		cancel event
		send "&4&lAntiBuild &6&l>> &cYou do not have permission to place blocks." to player
		
on drop:
	if player hasn't permission "antibuild.drop":
		cancel event
		send "&4&lAntiBuild &6&l>> &cYou do not have permission to drop items." to player
		
on damage:
	if attacker hasn't permission "antibuild.damage":
		cancel event
		send "&4&lAntiBuild &6&l>> &cYou do not have permission to hurt entities." to player