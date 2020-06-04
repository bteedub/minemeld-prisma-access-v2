# minemeld-prisma-access-v2

MineMeld Miner for Prisma Access API - Updated to use the v2 API

Almost all of this code is branched from the Palo Alto Network Prisma Access Miner work that Luigi Mori had already done.  The minor tweaks/changes involved adding payload for the v2 api, changing the request from a get to a post, and minor changes to Parsing the returned JSON.

# How To Install

1. Go to System > Extensions
2. Click on the git button (bottom right)
3. Paste https://github.com/bteedub/minemeld-prisma-access-v2.git in the URL field
4. Click Retrieve
5. Select the latest release
6. Click Install
7. Click Activate on the installed extension

NOTE:  IN ORDER TO HAVE THIS WORK, IT CURRENTLY PULLS THE API KEY FROM A SIDE_CONFIG FILE.  THE SIDE CONFIG FILE SHOULD BE IN YML FORMAT IN THE /opt/minemeld/local/config DIRECTORY, WITH THE FILE NAME BEING NODE-NAME_side_config.yml.  FOR EXAMPLE, IF YOUR NODE NAME IS lab-prisma-miner, THEN THE SIDE CONFIG SHOULD BE NAMED /opt/minemeld/local/config/lab-prisma-miner_side_config.yml.

NOTE:  CURRENTLY THE VERIFY SSL OPTIONS IS HARDCODED TO FALSE, AN UPDATE IS PLANNED TO OBEY THE OPTIONS IN THE SIDE_CONFIG FILE.

THE FILE SHOULD BE FORMATTED AS FOLLOWS:
<pre>
{
api_keys: ["API-KEY-HERE"]
}
</pre>
Thanks @bteedub
