```cs
enum StructureName {
	SmallHouse,
	LargeHouse,
	SmallShed, 
	LargeShed,
}

public class Structure {
	public StructureName Name;
	public Dictionary<Resource, int> _ingredients {get; private set;}
}
```

# Notes
- A base prefab will be created, with variants for each structure
- Base prefab will contain the script, a sprite, and a collision shape
- Variants will have these components set up correctly
- StructureBuilder will have an array of prefabs populated from Resources.load()
- 