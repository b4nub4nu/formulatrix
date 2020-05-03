# Purpose 
A Formulatrix repository manager is a library that can be used to store and retrieve JSON string or XML string. A unique string is used to indicate the item being stored.

# How to Run Test with xUnit ( dotnet CLI )

Open your terminal;

> git clone https://github.com/b4nub4nu/formulatrix.git

> cd formulatrix

> dotnet build Formulatrix.sln 

> cd xUnitTest

> dotnet test


# List Of xUnitTest

[Theory]

[InlineData("item1", "{\"name\":\"banu\",\"email\":\"banu.hutomo@gmail.com\",\"contents\":\"test formulatrix\"}", 1)]
[InlineData("item2", "<name>banu</name><email>banu.hutomo@gmail.com</email><contents>test formulatrix</contents>", 2)]

ReturnTrue_GivenParameters_RegisteringJSONXML

[Fact]

ReturnFalse_GivenDuplicatedItemNameAndItemType_RegisteringJSON

ReturnFalse_GivenDuplicatedItemNameAndItemType_RegisteringXML

ReturnFalse_GivenNoInputParameters_Registering

Return1_GivenitemName_getType

Return2_GivenitemName_getType

Return0_GivenitemNameWrong_getType

ReturnStringXML_GivenitemName_Retrieve

ReturnStringJson_GivenitemName_Retrieve

ReturnStringEmpty_GivenitemNameWrong_Retrieve

Deregister_GivenitemName

