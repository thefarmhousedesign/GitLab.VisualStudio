# GitLab  Extension for Visual Studio

You can log any of your favorite GitLab servers and start your great job!

The GitLab Extension for Visual Studio provides GitLab integration in Visual Studio 2015/2017.
Most of the extension UI lives in the Team Explorer pane, which is available from the View menu.

Appveyor:[![Build status](https://ci.appveyor.com/api/projects/status/qb510idi1wca2vet/branch/master?svg=true)](https://ci.appveyor.com/project/MaiKeBing/gitlab-visualstudio/branch/master)

The Visual Studio Extension is also available at the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=MysticBoy.GitLabExtensionforVisualStudio), or by searching for GitLab4VS  in the Visual Studio extension manager.
The latest build of the Visual Studio Extension is available at the [Open VsixGallery](http://vsixgallery.com/extension/54803a44-49e0-4935-bba4-7d7d91682273/)

[![Join the chat at https://gitter.im/GitLab-VisualStudio/](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/GitLab-VisualStudio?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)



### When you login with a user name and password.
  
For the new version of Gitlab：
1. https//gitlab.com or your GitLab server 
1. input your email address or username 
1. your password (not the token)
1. use "GitLab ApiV4 Oauth2" don't use "API v4" as the  instructions direct
1. Two-Factor : Off

For older versions of Gitlab
1. Your GitLab server 
1. input your email address or username 
1. your password (not the token)
1.use "GitLab ApiV3 Oauth2"  or  "API v3" 


***by Brett Winters***


### When you login with  2FA :

1) In GitLab, [top right] go to Settings then Access Tokens (left menu)
2) Enter a name & expire time (optional).
3) Check off "api" as the scope.
4) Click "Create Personal Access Token". This will appear in a textbox at the TOP of the page.
5) In Visual Studio, click "Connect" beside GitLab.
6) Enter your GitLab Username and paste in the Access Token.
7) Change it to "API v4" instead of "API v4 OAUTH2". 
8) Make sure "Two Factor Authentication" is CHECKED.
9) Save. You're DONE.

### When you login with  LDAP credentials :
If you create a personal access token (https://yourgitlaburl.com/profile/personal_access_tokens) and select 2fa and use your ldap username + your PAT you will be able to login and use the plug-in.

***by  dominicdejacomo***


## What's new ?

**V1.0.189** 
* Fix Groups and Subgroups missing in Namespace [#53](https://github.com/maikebing/GitLab.VisualStudio/issues/53)
* Fix Exception on Project Create [#52](https://github.com/maikebing/GitLab.VisualStudio/issues/52)

***Thanks [Rennerdo30](https://github.com/Rennerdo30)*** 


**V1.0.183**

* Fix for " cannot connect to custom gitlab server with different port [#50](https://github.com/maikebing/GitLab.VisualStudio/issues/50)

**V1.0.160**

* Automatically detects the API version of Gitlab

**V1.0.156**

* Visual Studio 2019 support

**V1.0.150** 

   - AddOpen URL from clipboard
   - Support Gitee.com 
   - fix #35

**V1.0.0.122**

Fix HttpUtility.UrlEncode processing username or email causing problems that cannot be logged in

**V1.0.0.119**

Now update login mode is OAuth2, which can't be logon before because the new version of GitLab's API session has been discarded.

The two API login methods are supported in the login interface, and the old version of GitLab needs to be selected manually. The default is that the login mode is OAuth2 and V4 !


**V1.0.0.115**

1.You can select GitLab Api version .

**V1.0.0.112**

1.modify "Open On GitLab" to "GitLab"

**V1.0.0.95**

1. French, Japanese, German and other languages have been added, but these are Google's translations, so we need human translation!
2. Open on GitLab move to  submenu!
3. Fixed issue #3,Thanks luky92!
4. The selected code can create code snippets directly
5. When you create a project, you can select namespases.
6. GitLab's Api is updated from V3 to V4.


**V1.0.0.70**

1. GitLab login information associated with the solution, easy to switch GitLab server.
2. Enter the password and press enter to login GitLab server.
3. Now, We can login   with two  factor authentication.just enter the personal access token into the password field.

**V1.0.0.58** 

1. Support for Visual Studio 2017 
2. Fix bus.


**V1.0.0.40** 
 1. Right click on editor, if repository is hosted on GitLab Server , you can jump to master/current branch/current revision's blob page and blame/commits page. If selecting line(single, range) in editor, jump with line number fragment.
 2. Fix [#4](https://www.gitlab.com/maikebing/GitLab.VisualStudio/issues/4) [#5](https://www.gitlab.com/maikebing/GitLab.VisualStudio/issues/5) [#6](https://www.gitlab.com/maikebing/GitLab.VisualStudio/issues/6)
Official builds of this extension are available at [the official website](http://visualstudio.gitclub.cn).

**HomePage**
 http://visualstudio.gitclub.cn/

### BUG And Issues

https://github.com/maikebing/GitLab.VisualStudio/issues

###    Visual Studio    |   Marketplace
https://marketplace.visualstudio.com/items?itemName=MysticBoy.GitLabExtensionforVisualStudio

### Thanks

####  GitHub Extension for Visual Studio

####  CodeCloud Extension for  Visual Studio

https://gitee.com/GitGroup/CodeCloud.VisualStudio

#### Visual Studio Extension for opening files on GitHub.com
https://github.com/neuecc/Open-on-GitHub 

#### NGitLab
https://github.com/Xarlot/NGitLab
https://github.com/Franklin89/NGitLab
https://github.com/maikebing/NGitLab



### Open On GitLab

![image](./docs/images/OpenOnGitLab.png)
###  Team Home Page

![image](./docs/images/TeamHome.PNG)

### Team Connct Page
![image](./docs/images/TeamConnect.PNG)

[![image](http://s07.flagcounter.com/map/7uzT/size_s/txt_000000/border_CCCCCC/pageviews_0/viewers_0/flags_0/)](http://info.flagcounter.com/7uzT)
[![image](http://ia.51.la/go1?id=19858017&pvFlag=1)](https://www.51.la/?19858017)

 
