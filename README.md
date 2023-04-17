# The-Internet-Folks

Due to security resons password removed from server.js file for testing please use this link https://snowflake-rose.vercel.app and below mentioned endpoints

<div class="sc-fzoKki kNKLJw"><div class="sc-fzpans vBDne"><span>
</span><span>
</span><span>
</span><h3 class="sc-fznKkj cJJIEu"><span>User Stories (Features)</span></h3><span>
</span><ul class="sc-fzpjYC XZKlG"><span>
</span><li><span>Module: Authentication</span><ul class="sc-fzpjYC XZKlG"><span>
</span><li><span>Feature: User should be able to signup using valid name, email and strong password.</span></li><span>
</span><li><span>Feature: User should be able to signin using valid credentials.</span></li><span>
</span></ul><span>
</span></li><span>
</span><li><span>Module: Community</span><ul class="sc-fzpjYC XZKlG"><span>
</span><li><span>Feature: User should be able to see all communities.</span></li><span>
</span><li><span>Feature: User should be able to create a community.</span></li><span>
</span></ul><span>
</span></li><span>
</span><li><span>Module: Moderation</span><ul class="sc-fzpjYC XZKlG"><span>
</span><li><span>Feature: User should be able to see all community members.</span></li><span>
</span><li><span>Feature: User should be able to add a user as member.</span></li><span>
</span><li><span>Feature: User should be able to remove a member from community.</span></li><span>
</span></ul><span>
</span></li><span>
</span></ul><span>
</span><h3 class="sc-fznKkj cJJIEu"><span>Problem Statement</span></h3><span>
</span><ul class="sc-fzpjYC XZKlG"><span>
</span><li><span>You need to build the APIs that adheres to above user stories.</span></li><span>
</span><li><span>The Role names are strict.</span></li><span>
</span><li><span>The API URLs and Response Structure is fixed.</span></li><span>
</span><li><span>The field attributes and table names are strict as well.</span></li><span>
</span><li><span>Addition of field for storing IDs when using NoSQL is allowed.</span></li><span>
</span><li><span>Validations for each API must be carried out.</span></li><span>
</span></ul><span>


</span><h2 class="sc-fznyAO eoTqIm"><span>Models</span></h2><span>
</span><h3 class="sc-fznKkj cJJIEu"><span>Architecture</span></h3><span>
</span><p><a class="sc-fznxKY gLMLqX markdown-link" href="https://postimg.cc/WtBfpLCy" target="_blank" rel="noreferrer noopener nofollow"></a></p><span>
</span><div class="sc-fzpmMD fkQxtr"><img src="https://i.postimg.cc/yYxqP7P7/Hiring-Assignment.png"></div><span>

</span><h3 class="sc-fznKkj cJJIEu"><span>User (</span><code><span>user</span></code><span>)</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Key</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Kind</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Notes</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>id</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>primary key</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>name</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>varchar(64)</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>default: null</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>email</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>varchar(128)</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>unique</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>password</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>varchar(64)</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>created_at</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>datetime</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><h3 class="sc-fznKkj cJJIEu"><span>Community (</span><code><span>community</span></code><span>)</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Key</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Kind</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Notes</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>id</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>primary key</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>name</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>varchar</span></code><span>(128)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>slug</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>varchar</span></code><span>(255)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>unique</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>owner</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>ref: &gt; </span><code><span>user.id</span></code><span>, relationship: </span><code><span>m2o</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>created_at</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>datetime</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>updated_at</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>datetime</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><h3 class="sc-fznKkj cJJIEu"><span>Role (</span><code><span>role</span></code><span>)</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Key</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Kind</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Notes</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>id</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>primary key</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>name</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>varchar(64)</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>unique</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>created_at</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>datetime</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>updated_at</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>datetime</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><h3 class="sc-fznKkj cJJIEu"><span>Member (</span><code><span>member</span></code><span>)</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Key</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Kind</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Notes</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>id</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>primary key</span></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>community</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>ref: &gt; </span><code><span>community.id</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>user</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>ref: &gt; </span><code><span>user.id</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>role</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>string</span></code><span> (snowflake)</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>ref: &gt; </span><code><span>role.id</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>created_at</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>datetime</span></code></td><span>
</span><td class="sc-fzqNqU cvBnEl"><span>-</span></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><p><span>Note:</span><br><span>Snowflake IDs are just string. Think of them just like UUID. Use our </span><a class="sc-fznxKY gLMLqX markdown-link" href="https://npmjs.com/package/@theinternetfolks/snowflake" target="_blank" rel="noreferrer noopener nofollow"><span>library</span></a><span> to generate unique Snowflake IDs . It works exactly like generating UUIDs.</span></p><span>
</span><h2 class="sc-fznyAO eoTqIm"><span>API Endpoints</span></h2><span>
</span><h3 class="sc-fznKkj cJJIEu"><span>Role</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Name</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>URL</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Create</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>POST /v1/role</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Get All</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>GET /v1/role</span></code></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><h3 class="sc-fznKkj cJJIEu"><span>User</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Name</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>URL</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Sign Up</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>POST /v1/auth/signup</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Sign in</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>POST /v1/auth/signin</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Get Me</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>GET /v1/auth/me</span></code></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><h3 class="sc-fznKkj cJJIEu"><span>Community</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Name</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>URL</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Create</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>POST /v1/community</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Get All</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>GET /v1/community</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Get All Members</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>GET /v1/community/:id/members</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Get My Owned Community</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>GET /v1/community/me/owner</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Get My Joined Community</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>GET /v1/community/me/member</span></code></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><h3 class="sc-fznKkj cJJIEu"><span>Member</span></h3><span>
</span><div class="click-to-expand-wrapper is-table-wrapper"><div class="sc-AxirZ iUfzzu"><table class="sc-fzoiQi kWlhWI"><span>
</span><thead><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><th class="sc-fzqARJ hIlZxG"><span>Name</span></th><span>
</span><th class="sc-fzqARJ hIlZxG"><span>URL</span></th><span>
</span></tr><span>
</span></thead><span>
</span><tbody><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Add Member</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>POST /v1/member</span></code></td><span>
</span></tr><span>
</span><tr class="sc-fzoyTs dAmCcp"><span>
</span><td class="sc-fzqNqU cvBnEl"><span>Remove Member</span></td><span>
</span><td class="sc-fzqNqU cvBnEl"><code><span>DELETE /v1/member/:id</span></code></td><span>
</span></tr><span>
</span></tbody><span>
</span></table></div><span>
</span></div><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span><span>
</span></div></div>
