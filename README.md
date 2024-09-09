local TestTable = {
	Bool = true,
	Number = 123,
	String = "Hello",
	Color = Color3.fromRGB(255, 255, 255),
	InnerTable = {
		Color2 = Color3.fromRGB(150, 150, 150),
		InnerInnerTable = {
			Color3_ = Color3.fromRGB(100, 100, 100),
			Vector3_ = Vector3.new(50, 200, 100),
			Vector2_ = Vector2.new(10, 20),
			InnerInnerInnerTable = {
				Key = Enum.KeyCode.X
			}
		}
	}
}

ConfigLibrary:Recursive(TestTable, warn)
