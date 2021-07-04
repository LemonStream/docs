## Description

Object used to get information about your current target.

## Forms

-   *target* **Target**

## Access to Types

-   *target* **target**
-   *[spawn](../data-types/datatype-spawn.md)* **spawn**

## Examples

-   To display the target's unique name as sent by EQ use ${Target} or ${Target.Name}

`/echo ${Target} or /echo ${Target.Name}`

  
*This will return "a_commander01" on a living mob or "a_commander's_corpse0" on a dead mob.*

------------------------------------------------------------------------------------------------------------------------

-   To display the target's clean name (also similar to %t on living mobs) use ${Target.CleanName} or
    ${Target.DisplayName}

`/echo ${Target.CleanName} or /echo ${Target.DisplayName}`

  
*This will return "a commander" on a living mob or "a commander's corpse" on a dead mob.*

------------------------------------------------------------------------------------------------------------------------

-   To display the name as used by '%t' on a corpse use the ${Target.DisplayName}

`/echo ${Target.DisplayName}`

  
*This will return "a commander" when the corpse is targetted.*

------------------------------------------------------------------------------------------------------------------------

-   To display the spell ID of the snare debuff use ${Target.Snared.ID}

`/echo ${Target.Snared.ID}`

------------------------------------------------------------------------------------------------------------------------

-   Example of using new Slowed target datatype

`/echo ${Target.Slowed.Name} will fade in ${Target.Slowed.Duration.TotalSeconds}s`

  
returns "\[MQ2\] Tepid Deeds will fade in 114s"

------------------------------------------------------------------------------------------------------------------------

-   Example of using new Mezzed target datatype

`/echo ${Target} will break mezz in ${Target.Mezzed.Duration.TotalSeconds}s`

  
returns "\[MQ2\] a_pyre_beetle48 will break mezz in 66s"

------------------------------------------------------------------------------------------------------------------------

## See Also

-   [Target](../commands/target.md)
-   [Top-Level Objects](top-level-objects.md)
-   [DataType:spawn](../data-types/datatype-spawn.md)
-   DataType:targettype

