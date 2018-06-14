<span data-ttu-id="601b9-101">运行标识基架：</span><span class="sxs-lookup"><span data-stu-id="601b9-101">Run the Identity scaffolder:</span></span>

# <a name="visual-studiotabvisual-studio"></a>[<span data-ttu-id="601b9-102">Visual Studio</span><span class="sxs-lookup"><span data-stu-id="601b9-102">Visual Studio</span></span>](#tab/visual-studio)

* <span data-ttu-id="601b9-103">从**解决方案资源管理器**，右键单击该项目 >**添加** > **新建基架项**。</span><span class="sxs-lookup"><span data-stu-id="601b9-103">From **Solution Explorer**, right-click on the project > **Add** > **New Scaffolded Item**.</span></span>
* <span data-ttu-id="601b9-104">从左窗格**添加基架**对话框中，选择**标识** > **添加**。</span><span class="sxs-lookup"><span data-stu-id="601b9-104">From the left pane of the **Add Scaffold** dialog, select **Identity** > **ADD**.</span></span>
* <span data-ttu-id="601b9-105">在**添加标识**对话框中，选择所需的选项。</span><span class="sxs-lookup"><span data-stu-id="601b9-105">In the **ADD Identity** dialog, select the options you want.</span></span>
  * <span data-ttu-id="601b9-106">选择现有的布局页上，或不正确的标记将被覆盖布局文件。</span><span class="sxs-lookup"><span data-stu-id="601b9-106">Select your existing layout page, or your layout file will be overwritten with incorrect markup.</span></span> <span data-ttu-id="601b9-107">选择现有 _Layout.cshtml 文件时，它是**不**覆盖。</span><span class="sxs-lookup"><span data-stu-id="601b9-107">When an existing _Layout.cshtml file is selected, it is **not** overwritten.</span></span>

 <span data-ttu-id="601b9-108">例如`~/Pages/Shared/_Layout.cshtml`Razor 页`~/Views/Shared/_Layout.cshtml`对于 MVC 项目</span><span class="sxs-lookup"><span data-stu-id="601b9-108">For example `~/Pages/Shared/_Layout.cshtml` for Razor Pages `~/Views/Shared/_Layout.cshtml` for MVC projects</span></span>
* <span data-ttu-id="601b9-109">若要使用你现有的数据上下文，选择要重写的至少一个文件。</span><span class="sxs-lookup"><span data-stu-id="601b9-109">To use your existing data context, select at least one file to override.</span></span> <span data-ttu-id="601b9-110">必须选择至少一个文件以添加你的数据上下文。</span><span class="sxs-lookup"><span data-stu-id="601b9-110">You must select at least one file to add your data context.</span></span>
  * <span data-ttu-id="601b9-111">选择您的数据上下文类。</span><span class="sxs-lookup"><span data-stu-id="601b9-111">Select your data context class.</span></span>
  * <span data-ttu-id="601b9-112">选择**添加**。</span><span class="sxs-lookup"><span data-stu-id="601b9-112">Select **ADD**.</span></span>
* <span data-ttu-id="601b9-113">若要创建新的用户上下文，并可能对标识创建自定义用户类：</span><span class="sxs-lookup"><span data-stu-id="601b9-113">To create a new user context and possibly create a custom user class for Identity:</span></span>
  * <span data-ttu-id="601b9-114">选择**+** 按钮以创建一个新**数据上下文类**。</span><span class="sxs-lookup"><span data-stu-id="601b9-114">Select the **+** button to create a new **Data context class**.</span></span>
  * <span data-ttu-id="601b9-115">选择**添加**。</span><span class="sxs-lookup"><span data-stu-id="601b9-115">Select **ADD**.</span></span>

<span data-ttu-id="601b9-116">注意： 如果你要创建新的用户上下文，你无需选择要重写的文件。</span><span class="sxs-lookup"><span data-stu-id="601b9-116">Note: If you're creating a new user context, you don't have to select a file to override.</span></span>

# <a name="net-core-clitabnetcore-cli"></a>[<span data-ttu-id="601b9-117">.NET Core CLI</span><span class="sxs-lookup"><span data-stu-id="601b9-117">.NET Core CLI</span></span>](#tab/netcore-cli)

<span data-ttu-id="601b9-118">如果以前尚未安装 ASP.NET 基架，请立即进行安装：</span><span class="sxs-lookup"><span data-stu-id="601b9-118">If you have not previously installed the ASP.NET scaffolder, install it now:</span></span>

```cli
dotnet tool install -g dotnet-aspnet-codegenerator
```

<span data-ttu-id="601b9-119">添加对的包引用[Microsoft.VisualStudio.Web.CodeGeneration.Design](https://www.nuget.org/packages/Microsoft.VisualStudio.Web.CodeGeneration.Design/)到项目 (\*.csproj) 文件。</span><span class="sxs-lookup"><span data-stu-id="601b9-119">Add a package reference to [Microsoft.VisualStudio.Web.CodeGeneration.Design](https://www.nuget.org/packages/Microsoft.VisualStudio.Web.CodeGeneration.Design/) to the project (\*.csproj) file.</span></span> <span data-ttu-id="601b9-120">在项目目录中运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="601b9-120">Run the following command in the project directory:</span></span>

```cli
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
dotnet restore
```

<span data-ttu-id="601b9-121">运行以下命令以列出标识基架选项：</span><span class="sxs-lookup"><span data-stu-id="601b9-121">Run the following command to list the Identity scaffolder options:</span></span>

```cli
dotnet aspnet-codegenerator identity -h
```

<span data-ttu-id="601b9-122">在项目文件夹中，使用所需的选项运行标识基架。</span><span class="sxs-lookup"><span data-stu-id="601b9-122">In the project folder, run the Identity scaffolder with the options you want.</span></span> <span data-ttu-id="601b9-123">例如，若要安装过程中使用默认 UI 的标识和文件的最小的数，运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="601b9-123">For example, to setup identity with the default UI and the minimum number of files, run the following command.</span></span> <span data-ttu-id="601b9-124">使用你的数据库上下文的正确完全限定的名：</span><span class="sxs-lookup"><span data-stu-id="601b9-124">Use the correct fully qualified name for your DB context:</span></span>

```cli
dotnet aspnet-codegenerator identity -dc MyWeb.Data.ApplicationDbContext --files Account.Register
```

-------------