# UnrealEngine5 Build Scripts

As always, any suggestions about how to improve the code are wellcome, have a great day.

Pssst, take a look at the license, it'd make me happy if you did any of the things listed on the ``Personal suggestions`` section of it.

## Version 1.2 unssupported Fix

### How to use

#### Step 1

Copy the whole ``Workarounds`` namespace into your ``[name].Build.cs`` file under the existing code.

#### Step 2

Call the following code

```cs
Workarounds.BuildVersionWorkaround.ExecuteWorkaround(Target.ProjectFile.ToNormalizedPath());
```

Anywhere on the constructor of all the classes that extends from ``ModuleRules`` or ``TargetRules``

#### Step 3 

If you had issues with the version 1.2 unssupported they should be fixed automatically so you don't have to worry about them anymore

