# New Character Generator

```button
name Reload Rant
type command
action Rant-Lang: Re-rant with random seed (active file)
color default
```
^button-x9z0


```rant

# A selection to synchronize gender with pronouns and name endings
<$gendersync = [mksel:one]>

<$mark-custom = "<mark style="background-color:E7EAFF">">

# The Masculine name endings
[$masc]
{
	"`dice: [[Name Dice Tables#^masc]]`"
}

# The Feminine name endings
[$femme]
{
	"`dice: [[Name Dice Tables#^femme]]`"
}

# Classes that are magic based
[$magic-classes]
{
	{
		Cleric|Druid|Sorcerer|Warlock|Wizard
	}
}

[$physical-classes]
{
	{
		Barbarian|Fighter|Monk|Paladin|Blood Hunter
	}
}

[$skilled-classes]
{
	{
		Bard|Rogue|Artificer
	}
}

<@text $he-pro = (::
	they = "He";
	them = "Him";
	their = "His";
	isare = "is";
	themselves = "Himself";
	werewas = "was";
	plural = "s";
	)>
	
<@text $she-pro = (::
	they = "She";
	them = "Her";
	their = "Her";
	isare = "is";
	themselves = "Herself";
	werewas = "was";
	plural = "s";
	)>
	
<@text $they-pro = (::
	they = "They";
	them = "Them";
	their = "Their";
	isare = "are";
	themselves = "Themselves";
	werewas = "were";
	plural = \0;
	)>
	
<@text $xe-pro = (::
	they = "Xe";
	them = "Xem";
	their = "Xyr";
	isare = "is";
	themselves = "Xemself";
	werewas = "was";
	plural = "s";
	)>

<@text $pronouns = 
	[sel:<gendersync>]{
		<he-pro>|
		<she-pro>|
		<they-pro>|
		<xe-pro>
		}>

<@text $magic-jobs = (::
	class = [magic-classes];
	jobs = (:
		"Apothecary";
		"Astrologer";
		"Bottler";
		"Candlemaker";
		"Chamberlain";
		"Chancellor";
		"Clerk";
		"Constable";
		"Cook";
		"Gardener";
		"Herbalist";
		"Physician";
		"Scribe";
		"Scholar";
		"Witch";
		"Messenger";
		"Child")
	)>

<@text $physical-jobs = (::
	class = [physical-classes];
	jobs = (
		"Armorer";
		"Blacksmith";
		"Carpenter";
		"Knight";
		"Marshal";
		"Page";
		"Sheriff";
		"Child")
	)>

<@text $skilled-jobs = (::
	class = [skilled-classes];
	jobs = (:
		"Apothecary";
		"Artist";
		"Baker";
		"Barber";
		"Bottler";
		"Butler";
		"Candlemaker";
		"Carpenter";
		"Clerk";
		"Clothier";
		"Constable";
		"Cook";
		"Fletcher";
		"Gardener";
		"Jester";
		"Messenger";
		"Painter";
		"Physician";
		"Potter";
		"Shoemaker";
		"Child")
	)>

<$selected-job = {
	<magic-jobs>|
	<physical-jobs>|
	<skilled-jobs>
	}>


[$relationship-target: unestablished?]
	{
	<$selected-job = {
		<magic-jobs>|
		<physical-jobs>|
		<skilled-jobs>
		}>
	
	<$gendersync = [mksel:one]>
		@return {
		
			[if: <unestablished ? @true>]
				{
				
				"✧`dice: #dnd/npc|link`"|
				
				"✧`dice: #dnd/npc|link`"|
				
				"✧`dice: #dnd/factions|link`"|
				
				"✦`dice: [[Name Dice Tables#^names]]`"\0[sel:<gendersync>]{[masc]|[femme]|} 
				
				\("✦`dice: [[Race Dice Tables#^main]]`"
				
				 `[sel:<gendersync>] `{He\/Him|She\/Her|{They\/Them|Xe\/Xyr}} 
				
				`[pick:<selected-job/jobs>]\/<selected-job/class>\)
				}
				
			[else]
				{
				
				"✧`dice: #dnd/pc|link`"|
				
				"✧`dice: #dnd/npc|link`"
				
				}
		}
	}
	
	
[$relationship-opinion]
	{
		{
			and <pronouns/they> <pronouns/isare> out to get them|
			
			and <pronouns/they> admire<pronouns/plural> them|
			
			and <pronouns/they> fear<pronouns/plural> them|
			
			and <pronouns/they> hate<pronouns/plural> them|
			
			and <pronouns/they> would like to get closer to them|
			
			and <pronouns/they> personally consider<pronouns/plural> <pronouns/themselves> an old {friend|rival} of theirs|
			
			and they remind <pronouns/them> of someone near and dear to  <pronouns/their> heart 
		}
	}


[$relationship]
	{
		{
			{(Secretly)" "|}<pronouns/they> help<pronouns/plural>, aid<pronouns/plural>, or work<pronouns/plural> for `[relationship-target].|
			
			<pronouns/they> <pronouns/isare> `{ secretly|} out to get `[relationship-target].|
			
			<pronouns/they> `{secretly|} owe<pronouns/plural> `[relationship-target] some {great|major|minor|} debt.|
			
			<pronouns/they> <pronouns/isare> `{{ secretly and |} knowingly|unknowingly} obstructing `[relationship-target]'s goals.|
			
			<pronouns/they> <pronouns/isare> `{ secretly|} from `[relationship-target: @false]'s past `[relationship-opinion].|
			
			<pronouns/they> {secretly|} heard of `[relationship-target: @false] from tales {full of lies|of their deeds} and `[relationship-opinion].|
			
			`{(secretly) |} <pronouns/they> `{<pronouns/isare> |<pronouns/werewas> once } associated with "✧`dice: #dnd/factions|link`"
		}
	}














# The output!!








"## Basics"

\r\r"This character's name is" "✦`dice: [[Name Dice Tables#^names]]`"
	\0[sel:<gendersync>]{[masc]|[femme]|\0|\0}, <mark-custom>"**"`[sel:<gendersync>]{He\/Him|She\/Her|They\/Them|Xe\/Xyr}"**</mark>" 

\r\r <pronouns/they> <pronouns/isare> a(n) "✦`dice: [[Race Dice Tables#^main]]`" 
	<mark-custom> "**"`[pick:<selected-job/jobs>]"**</mark>". 
	
	They wear "✦`dice: [[Misc Dice Tables#^color-alt]]`" 
		clothes with "✦`dice: [[Misc Dice Tables#^color-alt]]`" accents.

\r\r [sel:<gendersync>] `{He is|She is|They are|Xe is} 
	"✦`dice: [[NPC Dice Tables#^personal-adj]]`" and  
	"✦`dice: [[NPC Dice Tables#^personal-adj]]`"



\r"## Additional"

\r <pronouns/they> <pronouns/isare> from {"✧`dice: #dnd/town|link`"|"✧`dice: #DND/Region|link`"}

\r\r If <pronouns/they> must take up arms, <pronouns/they> would be a <mark-custom>"**"<selected-job/class>"**</mark>".

\r\r <mark-custom>"**"[relationship]"**</mark>"

\r\r <pronouns/they> initially "✦`dice: [[NPC Dice Tables#^disposition]]`" towards the party.

\r\r <pronouns/their> goal is "✦`dice: [[NPC Dice Tables#^goals]]`"

\r\r <pronouns/they> recently experienced a "✦`dice: [[Misc Dice Tables#^events-alt]]`"






\r "## Personality Matrix"

<$value=[rand: 1; 10]>
\r\r+ Way of speaking ("**"<value>"**"\/"**"10"**")
\r\t+ "**Casual**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Formal**"

\r\r+ Appearence ("**"<value>"**"\/"**"10"**")
\r\t+ "**Unkempt**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Vain**"

<value=[rand: 1; 10]>
\r\r+ Ambition ("**"<value>"**"\/"**"10"**")
\r\t+ "**Lazy**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Obsessed**"

<value=[rand: 1; 10]>
\r\r+ Emotional Stability ("**"<value>"**"\/"**"10"**")
\r\t+ "**Unstable**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Stable**"

<value=[rand: 1; 10]>
\r\r+ Wisdom ("**"<value>"**"\/"**"10"**")
\r\t+ "**Naive**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Experienced**"

\r\r+ Judgement of Others ("**"<value>"**"\/"**"10"**")
\r\t+ "**Forgiving**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Hypercritical**"

<value=[rand: 1; 10]>
\r\r+ Sociability ("**"<value>"**"\/"**"10"**")
\r\t+ "**Antisocial**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Social Butterlfy**"

<value=[rand: 1; 10]>
\r\r+ Modesty ("**"<value>"**"/"**"10"**")
\r\t+ "**Humble**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Pridful**"

<value=[rand: 1; 10]>
\r\r+ Bravery ("**"<value>"**"\/"**"10"**")
\r\t+ "**Cowardly**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Rash**"


<value=[rand: 1; 10]>
\r\r+ Trust ("**"<value>"**"\/"**"10"**")
\r\t+ "**Skeptical**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Gullible**"

<value=[rand: 1; 10]>
\r\r+ Self Control ("**"<value>"**"\/"**"10"**")
\r\t+ "**Indescisive**" "<progress value="<value>" max=10 style="width:100px"></progress>" "**Impulsive**"




\r\r "## Tarot"

\r\r"<center><img src=""https://i.imgur.com/EyCAclD.png"" width=20%></img></center>"

\r\r These tarot cards are heavily associated with <pronouns/them>:
\r+ Overall card: "✦`dice: [[Tarot Dice Tables#^main]]`"
\r+ Fortune: "✦`dice: [[Tarot Dice Tables#^main-fortune]]`"
\r+ Keywords
\r\t+ "✦`dice: [[Tarot Dice Tables#^main-keywords]]`"
\r\t+ "✦`dice: [[Tarot Dice Tables#^main-keywords]]`"
\r\t+ "✦`dice: [[Tarot Dice Tables#^main-keywords]]`"


```




