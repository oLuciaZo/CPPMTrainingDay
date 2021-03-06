# CPPMTrainingDay

class ipv4 "IP-Any-Any"<BR>
10 match ip 0.0.0.0 255.255.255.255 0.0.0.0 255.255.255.255<BR>
exit<BR>
policy user "DS-User"<BR>
10 class ipv4 "IP-Any-Any" action permit<BR>
exit<BR>
aaa authorization user-role name "DS-User-Profiler-Role"<BR>
policy "DS-User"<BR>
tunneled-node-server-redirect secondary-role "Profiler"<BR>
exit<BR>


![image](https://user-images.githubusercontent.com/18340935/153616592-69444067-142a-44d6-af08-1e4e55f6f607.png)


Document and Materials

<a href="https://community.arubanetworks.com/community-home/digestviewer/viewthread?MessageKey=ee47602d-861e-407a-a269-1cd1f00725e0&CommunityKey=aa40c287-728e-4827-b062-5eff4ed6410b&tab=digestviewer&bm=ee47602d-861e-407a-a269-1cd1f00725e0#bmee47602d-861e-407a-a269-1cd1f00725e0">- Aruba CX Configuration Guide</a> 

<a href="https://community.arubanetworks.com/blogs/esupport1/2020/04/29/downloadable-user-role-configuration-in-aruba-os-cx-with-mac-authentication">- Clearpass DUR with Aruba CX</a> 

<a href="https://arubapedia.arubanetworks.com/arubapedia/index.php/File:ClearPassPoCKit_v6.7.zip">- Clearpass with Aruba Wireless PoC Kits</a> 

<a href="https://www.youtube.com/c/ABCNetworking/playlists?view=50&sort=dd&shelf_id=8">- Clearpass Video Tutorial</a> 

<a href="https://www.arubanetworks.com/techdocs/ClearPass/6.7/Aruba_DeployGd_HTML/Default.htm#About%20ClearPass/About_this_guide.htm%3FTocPath%3DAbout%2520ClearPass%7C_____1">- Clearpass Document Guide</a> 


Group Arrangement<BR>
Group1-4 IT Green<BR>
Group5-8 SIS<BR>
Group9-12 VST<BR>

LAB Switch Server<BR>
Group 1-4  10.5.255.50 (IT Green)<BR>
Group 5-8  10.5.255.51 (SIS)<BR>
Group 9-12 10.5.255.52 (VST)<BR>


Clearpass Server<BR>
Group 1-4  10.20.22.201 (IT Green)<BR>
Group 5-8  10.20.22.202 (SIS)<BR>
Group 9-12 10.20.22.203 (VST)<BR>


<img width="735" alt="image" src="https://user-images.githubusercontent.com/18340935/154606909-34cce3d1-1b35-4452-9c57-1e4ee97ea44c.png">
<img width="1127" alt="image" src="https://user-images.githubusercontent.com/18340935/154606944-74a395cb-02ec-4a9d-904c-7ac0d56acecf.png">


