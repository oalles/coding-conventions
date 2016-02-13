## Coding Conventions

I will use UTF-8 and Unix style line delimiters.

Eclipse *save actions* in order to Format(ctrl-shift-F) and Organize Imports (ctrl-shift-O).

###Eclipse Setup

1. Text File Encoding

	+	Workspace-wide: Window->Preferences->General->Workspace
		```
		Text File Encoding, Other: UTF-8
		``` 
	+ Project specific: Properties->Resource
		```
		Text File Encoding, Other: UTF-8
		```

2. Formatting

	Coding convention preferences can be set either as a workspace (preferred) or project preference.

	+	Window->Preferences->Java->Code style->Clean Up->Import cleanup.xml
	+	Window->Preferences->Java->Code style->Formatter->javaconventions.xml
	+	Window->Preferences->Java->Editor->Save Actions
			[x] Perform the selected actions ...
			[x] Format
			[x] Organize imports
			[x] Additional actions -> Configure

					+ Code Organizing tab: Select Remove trailing whitespace for All lines, deselect everything else

					+ Code Style tab: Select Use blocks in... Always, deselect everything else

					+ Member Accesses tab: On both Use 'this'..., select Only if necessary, deselect everything else

					+ Missing Code tab: Select everything except Implementations of interface methods (1.6 or higher)

					+ Unnecessary Code tab: Select Remove unused importas and Remove unnecessary casts, deselect everything else

					+ Press OK to close the Additional Save Actions dialog

			The list of Additional actions should now contain these entries

					+ Remove 'this' qualifier for non static field accesses

					+ Remove 'this' qualifier for non static method accesses

					+ Convert control statement bodies to block

					+ Remove unused imports

					+ Add missing '@Override' annotations

					+ Add missing '@Deprecated' annotations

					+ Remove unnecessary casts

					+ Remove trailing whitespace on all lines

	+	Window->Preferences->Java->Compiler->Error/Warnings

			Set "Potential Programming Problems->Serializable class without SerializableUID" to ignore

	+	General -> Workspace

			Set "New text file delimiter" to "Other: Unix"
			
Read:

	[java coding conventions](http://www.oracle.com/technetwork/java/codeconventions-150003.pdf)

	[google java style](https://google.github.io/styleguide/javaguide.html)