----Commands to write code and test reference
dotnet new webapi -n SimpleAPI
dotnet new xunit -n SimpleAPI.Tests
dotnet new sln --name SimpleAPI
dotnet sln SimpleAPI.sln add src/SimpleAPI/SimpleAPI.csproj test/SimpleAPI.Tests/SimpleAPI.Tests.csproj
dotnet add test/SimpleAPI.Tests/SimpleAPI.Tests.csproj reference src/SimpleAPI/SimpleAPI.csproj

we are implementing CI/CD
-- test application is taking beifit of .net core


-- added xunit package

way to add refrence of project


<ItemGroup>
    <ProjectReference Include="..\..\src\SimpleAPI\SimpleAPI.csproj" />
  </ItemGroup>
--  <ProjectReference Include="..\..\src\SimpleAPI\SimpleAPI.csproj" /> 


Test case run on AAA pattern
- Arrange
- Act
- Assert --- (this is inbuilt calss.. it has all functions -- )


MOCK AND 
MOQ Library -- this will create a clone of project to test all in local