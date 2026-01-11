# Reference
## Auth
<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">register</a>(...) -> AsyncHttpResponse[PostAuthRegisterResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.auth.register(
    username="username",
    email="email",
    password="password",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**username:** `str` — Username
    
</dd>
</dl>

<dl>
<dd>

**email:** `str` — Email
    
</dd>
</dl>

<dl>
<dd>

**password:** `str` — Password (min 8 chars)
    
</dd>
</dl>

<dl>
<dd>

**display_name:** `typing.Optional[str]` — Display Name
    
</dd>
</dl>

<dl>
<dd>

**roles:** `typing.Optional[typing.Sequence[str]]` — Roles
    
</dd>
</dl>

<dl>
<dd>

**bio:** `typing.Optional[str]` — Bio
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">login</a>(...) -> AsyncHttpResponse[PostAuthLoginResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.auth.login(
    login="login",
    password="password",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**login:** `str` — Username or Email
    
</dd>
</dl>

<dl>
<dd>

**password:** `str` — Password
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">get_current_user</a>() -> AsyncHttpResponse[GetAuthMeResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.auth.get_current_user()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">request_password_reset</a>(...) -> AsyncHttpResponse[PostAuthForgotPasswordResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.auth.request_password_reset(
    email="email",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**email:** `str` — User Email
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">reset_password</a>(...) -> AsyncHttpResponse[PostAuthResetPasswordResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.auth.reset_password(
    password="password",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**password:** `str` — New Password (min 8 chars)
    
</dd>
</dl>

<dl>
<dd>

**old_password:** `typing.Optional[str]` — Old Password (for change password)
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` — Email (required if using oldPassword)
    
</dd>
</dl>

<dl>
<dd>

**token:** `typing.Optional[str]` — Reset Token
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Tags
<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">list_all_tags</a>(...) -> AsyncHttpResponse[GetTagsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.list_all_tags()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">create_a_tag</a>(...) -> AsyncHttpResponse[PostTagsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.create_a_tag(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` — Tag name
    
</dd>
</dl>

<dl>
<dd>

**slug:** `typing.Optional[str]` — Tag slug (unique identifier)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Tag description
    
</dd>
</dl>

<dl>
<dd>

**color:** `typing.Optional[str]` — Hex color code
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">get_a_tag</a>(...) -> AsyncHttpResponse[GetTagsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.get_a_tag(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">delete_a_tag</a>(...) -> AsyncHttpResponse[DeleteTagsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.delete_a_tag(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">update_a_tag</a>(...) -> AsyncHttpResponse[PatchTagsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.update_a_tag(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` — Tag name
    
</dd>
</dl>

<dl>
<dd>

**slug:** `typing.Optional[str]` — Tag slug (unique identifier)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Tag description
    
</dd>
</dl>

<dl>
<dd>

**color:** `typing.Optional[str]` — Hex color code
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">list_tag_subscribers</a>(...) -> AsyncHttpResponse[GetTagsIdSubscribersResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.list_tag_subscribers(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Tag ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">get_a_subscriber_from_tag</a>(...) -> AsyncHttpResponse[GetTagsIdSubscribersSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.get_a_subscriber_from_tag(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Tag ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Subscriber ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">delete_a_subscriber_from_tag</a>(...) -> AsyncHttpResponse[DeleteTagsIdSubscribersSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.tags.delete_a_subscriber_from_tag(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Tag ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Subscriber ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Threads
<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_all_threads</a>(...) -> AsyncHttpResponse[GetThreadsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.list_all_threads()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">create_a_thread</a>(...) -> AsyncHttpResponse[PostThreadsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.create_a_thread(
    title="title",
    body="body",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**title:** `str` — Thread title
    
</dd>
</dl>

<dl>
<dd>

**body:** `str` — Thread content (Markdown supported)
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Author user ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**tags:** `typing.Optional[typing.Sequence[str]]` — List of tag slugs, names, or IDs to attach
    
</dd>
</dl>

<dl>
<dd>

**poll:** `typing.Optional[PostThreadsRequestPoll]` — Poll data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">get_a_thread</a>(...) -> AsyncHttpResponse[GetThreadsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.get_a_thread(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_a_thread</a>(...) -> AsyncHttpResponse[DeleteThreadsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.delete_a_thread(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">update_a_thread</a>(...) -> AsyncHttpResponse[PatchThreadsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.update_a_thread(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` — New title
    
</dd>
</dl>

<dl>
<dd>

**body:** `typing.Optional[str]` — New content
    
</dd>
</dl>

<dl>
<dd>

**locked:** `typing.Optional[bool]` — Lock/unlock thread
    
</dd>
</dl>

<dl>
<dd>

**pinned:** `typing.Optional[bool]` — Pin/unpin thread
    
</dd>
</dl>

<dl>
<dd>

**tags:** `typing.Optional[typing.Sequence[str]]` — Update tags by slug, name, or ID
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Update extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_thread_posts</a>(...) -> AsyncHttpResponse[GetThreadsIdPostsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.list_thread_posts(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">get_a_post_from_thread</a>(...) -> AsyncHttpResponse[GetThreadsIdPostsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.get_a_post_from_thread(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_a_post_from_thread</a>(...) -> AsyncHttpResponse[DeleteThreadsIdPostsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.delete_a_post_from_thread(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_thread_reactions</a>(...) -> AsyncHttpResponse[GetThreadsIdReactionsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.list_thread_reactions(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">create_a_reaction_in_thread</a>(...) -> AsyncHttpResponse[PostThreadsIdReactionsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.create_a_reaction_in_thread(
    id="id",
    type="LIKE",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**type:** `PostThreadsIdReactionsRequestType` — Type of reaction
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — User ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Additional custom data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">remove_your_reaction_from_thread</a>(...) -> AsyncHttpResponse[DeleteThreadsIdReactionsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the authenticated user's reaction. No subId needed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.remove_your_reaction_from_thread(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">get_a_reaction_from_thread</a>(...) -> AsyncHttpResponse[GetThreadsIdReactionsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.get_a_reaction_from_thread(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Reaction ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_a_reaction_from_thread</a>(...) -> AsyncHttpResponse[DeleteThreadsIdReactionsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.delete_a_reaction_from_thread(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Reaction ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_thread_subscribers</a>(...) -> AsyncHttpResponse[GetThreadsIdSubscribersResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.list_thread_subscribers(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">get_a_subscriber_from_thread</a>(...) -> AsyncHttpResponse[GetThreadsIdSubscribersSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.get_a_subscriber_from_thread(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Subscriber ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_a_subscriber_from_thread</a>(...) -> AsyncHttpResponse[DeleteThreadsIdSubscribersSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.delete_a_subscriber_from_thread(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Subscriber ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">get_thread_poll</a>(...) -> AsyncHttpResponse[GetThreadsIdPollResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.get_thread_poll(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">create_thread_poll</a>(...) -> AsyncHttpResponse[PostThreadsIdPollResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient
from foru_ms_sdk.threads import PostThreadsIdPollRequestOptionsItem

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.create_thread_poll(
    id="id",
    title="title",
    options=[
        PostThreadsIdPollRequestOptionsItem(
            title="title",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**title:** `str` — Poll question/title
    
</dd>
</dl>

<dl>
<dd>

**options:** `typing.Sequence[PostThreadsIdPollRequestOptionsItem]` — Poll options (2-20)
    
</dd>
</dl>

<dl>
<dd>

**expires_at:** `typing.Optional[dt.datetime]` — Optional expiration time
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Additional custom data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">update_thread_poll</a>(...) -> AsyncHttpResponse[PatchThreadsIdPollResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.update_thread_poll(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Thread ID
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` — Poll question/title
    
</dd>
</dl>

<dl>
<dd>

**closed:** `typing.Optional[bool]` — Close the poll
    
</dd>
</dl>

<dl>
<dd>

**expires_at:** `typing.Optional[dt.datetime]` — Optional expiration time
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Additional custom data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Posts
<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">list_all_posts</a>(...) -> AsyncHttpResponse[GetPostsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.list_all_posts()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">create_a_post</a>(...) -> AsyncHttpResponse[PostPostsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.create_a_post(
    thread_id="threadId",
    body="body",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**thread_id:** `str` — Thread ID to post in
    
</dd>
</dl>

<dl>
<dd>

**body:** `str` — Post content (Markdown supported)
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Author user ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` — Parent post ID for threading
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">get_a_post</a>(...) -> AsyncHttpResponse[GetPostsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.get_a_post(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">delete_a_post</a>(...) -> AsyncHttpResponse[DeletePostsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.delete_a_post(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">update_a_post</a>(...) -> AsyncHttpResponse[PatchPostsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.update_a_post(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**body:** `typing.Optional[str]` — Updated post content
    
</dd>
</dl>

<dl>
<dd>

**thread_id:** `typing.Optional[str]` — Move post to another thread
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` — Change parent post
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Update extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">list_post_reactions</a>(...) -> AsyncHttpResponse[GetPostsIdReactionsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.list_post_reactions(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">create_a_reaction_in_post</a>(...) -> AsyncHttpResponse[PostPostsIdReactionsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.create_a_reaction_in_post(
    id="id",
    type="LIKE",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**type:** `PostPostsIdReactionsRequestType` — Type of reaction
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — User ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Additional custom data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">remove_your_reaction_from_post</a>(...) -> AsyncHttpResponse[DeletePostsIdReactionsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the authenticated user's reaction. No subId needed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.remove_your_reaction_from_post(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">get_a_reaction_from_post</a>(...) -> AsyncHttpResponse[GetPostsIdReactionsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.get_a_reaction_from_post(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Reaction ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">delete_a_reaction_from_post</a>(...) -> AsyncHttpResponse[DeletePostsIdReactionsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.delete_a_reaction_from_post(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Reaction ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">list_post_posts</a>(...) -> AsyncHttpResponse[GetPostsIdPostsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.list_post_posts(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">get_a_post_from_post</a>(...) -> AsyncHttpResponse[GetPostsIdPostsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.get_a_post_from_post(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">delete_a_post_from_post</a>(...) -> AsyncHttpResponse[DeletePostsIdPostsSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.posts.delete_a_post_from_post(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Post ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## PrivateMessages
<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">list_all_private_messages</a>(...) -> AsyncHttpResponse[GetPrivateMessagesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.list_all_private_messages()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">create_a_private_message</a>(...) -> AsyncHttpResponse[PostPrivateMessagesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.create_a_private_message(
    recipient_id="recipientId",
    body="body",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**recipient_id:** `str` — Recipient User ID
    
</dd>
</dl>

<dl>
<dd>

**body:** `str` — Message content
    
</dd>
</dl>

<dl>
<dd>

**sender_id:** `typing.Optional[str]` — Sender user ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` — Message title (optional for replies)
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` — Parent Message ID (for replies)
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">get_a_private_message</a>(...) -> AsyncHttpResponse[GetPrivateMessagesIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.get_a_private_message(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">delete_a_private_message</a>(...) -> AsyncHttpResponse[DeletePrivateMessagesIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.delete_a_private_message(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">list_private_message_replies</a>(...) -> AsyncHttpResponse[GetPrivateMessagesIdRepliesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.list_private_message_replies(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Private Message ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">create_a_reply_in_private_message</a>(...) -> AsyncHttpResponse[PostPrivateMessagesIdRepliesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.create_a_reply_in_private_message(
    id="id",
    recipient_id="recipientId",
    body="body",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Private Message ID
    
</dd>
</dl>

<dl>
<dd>

**recipient_id:** `str` — Recipient User ID
    
</dd>
</dl>

<dl>
<dd>

**body:** `str` — Message content
    
</dd>
</dl>

<dl>
<dd>

**sender_id:** `typing.Optional[str]` — Sender user ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` — Message title (optional for replies)
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` — Parent Message ID (for replies)
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">get_a_reply_from_private_message</a>(...) -> AsyncHttpResponse[GetPrivateMessagesIdRepliesSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.get_a_reply_from_private_message(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Private Message ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Reply ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">delete_a_reply_from_private_message</a>(...) -> AsyncHttpResponse[DeletePrivateMessagesIdRepliesSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.private_messages.delete_a_reply_from_private_message(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Private Message ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Reply ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Users
<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">list_all_users</a>(...) -> AsyncHttpResponse[GetUsersResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.list_all_users()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">get_a_user</a>(...) -> AsyncHttpResponse[GetUsersIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.get_a_user(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">delete_a_user</a>(...) -> AsyncHttpResponse[DeleteUsersIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.delete_a_user(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">update_a_user</a>(...) -> AsyncHttpResponse[PatchUsersIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.update_a_user(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**display_name:** `typing.Optional[str]` — Display name
    
</dd>
</dl>

<dl>
<dd>

**bio:** `typing.Optional[str]` — User bio
    
</dd>
</dl>

<dl>
<dd>

**signature:** `typing.Optional[str]` — Forum signature
    
</dd>
</dl>

<dl>
<dd>

**username:** `typing.Optional[str]` — Username (letters, numbers, underscores, hyphens)
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` — Email address
    
</dd>
</dl>

<dl>
<dd>

**password:** `typing.Optional[str]` — New password
    
</dd>
</dl>

<dl>
<dd>

**url:** `typing.Optional[str]` — Website URL
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**roles:** `typing.Optional[typing.Sequence[str]]` — Role slugs (admin only)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">list_user_followers</a>(...) -> AsyncHttpResponse[GetUsersIdFollowersResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.list_user_followers(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — User ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">get_a_follower_from_user</a>(...) -> AsyncHttpResponse[GetUsersIdFollowersSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.get_a_follower_from_user(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — User ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Follower ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">delete_a_follower_from_user</a>(...) -> AsyncHttpResponse[DeleteUsersIdFollowersSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.delete_a_follower_from_user(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — User ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Follower ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">list_user_following</a>(...) -> AsyncHttpResponse[GetUsersIdFollowingResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.list_user_following(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — User ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">get_a_following_from_user</a>(...) -> AsyncHttpResponse[GetUsersIdFollowingSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.get_a_following_from_user(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — User ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Following ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">delete_a_following_from_user</a>(...) -> AsyncHttpResponse[DeleteUsersIdFollowingSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.users.delete_a_following_from_user(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — User ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Following ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Roles
<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">list_all_roles</a>(...) -> AsyncHttpResponse[GetRolesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.roles.list_all_roles()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">create_a_role</a>(...) -> AsyncHttpResponse[PostRolesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.roles.create_a_role(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` — Role name
    
</dd>
</dl>

<dl>
<dd>

**slug:** `typing.Optional[str]` — Role slug (unique identifier)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Role description
    
</dd>
</dl>

<dl>
<dd>

**color:** `typing.Optional[str]` — Role color hex
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">get_a_role</a>(...) -> AsyncHttpResponse[GetRolesIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.roles.get_a_role(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">delete_a_role</a>(...) -> AsyncHttpResponse[DeleteRolesIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.roles.delete_a_role(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">update_a_role</a>(...) -> AsyncHttpResponse[PatchRolesIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.roles.update_a_role(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` — Role name
    
</dd>
</dl>

<dl>
<dd>

**slug:** `typing.Optional[str]` — Role slug (unique identifier)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Role description
    
</dd>
</dl>

<dl>
<dd>

**color:** `typing.Optional[str]` — Role color hex
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Reports
<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">list_all_reports</a>(...) -> AsyncHttpResponse[GetReportsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.reports.list_all_reports()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">create_a_report</a>(...) -> AsyncHttpResponse[PostReportsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.reports.create_a_report(
    type="type",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `str` — Report type (e.g. spam, abuse)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Reason for reporting
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Reporter user ID (required for API key auth, ignored for JWT auth)
    
</dd>
</dl>

<dl>
<dd>

**reported_id:** `typing.Optional[str]` — ID of user being reported
    
</dd>
</dl>

<dl>
<dd>

**thread_id:** `typing.Optional[str]` — ID of thread being reported
    
</dd>
</dl>

<dl>
<dd>

**post_id:** `typing.Optional[str]` — ID of post being reported
    
</dd>
</dl>

<dl>
<dd>

**private_message_id:** `typing.Optional[str]` — ID of private message being reported
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">get_a_report</a>(...) -> AsyncHttpResponse[GetReportsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.reports.get_a_report(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">delete_a_report</a>(...) -> AsyncHttpResponse[DeleteReportsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.reports.delete_a_report(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Notifications
<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">list_all_notifications</a>(...) -> AsyncHttpResponse[GetNotificationsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.notifications.list_all_notifications()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">create_a_notification</a>(...) -> AsyncHttpResponse[PostNotificationsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.notifications.create_a_notification(
    user_id="userId",
    type="type",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**user_id:** `str` — Target user ID to receive notification (maps to userId)
    
</dd>
</dl>

<dl>
<dd>

**type:** `str` — Notification type (e.g. mention, reply, follow)
    
</dd>
</dl>

<dl>
<dd>

**notifier_id:** `typing.Optional[str]` — User ID who triggered the notification (optional, defaults to authenticated user)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Notification text content
    
</dd>
</dl>

<dl>
<dd>

**thread_id:** `typing.Optional[str]` — Related thread ID
    
</dd>
</dl>

<dl>
<dd>

**post_id:** `typing.Optional[str]` — Related post ID
    
</dd>
</dl>

<dl>
<dd>

**private_message_id:** `typing.Optional[str]` — Related private message ID
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[PostNotificationsRequestStatus]` — Initial notification status
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Additional notification data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">get_a_notification</a>(...) -> AsyncHttpResponse[GetNotificationsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.notifications.get_a_notification(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">delete_a_notification</a>(...) -> AsyncHttpResponse[DeleteNotificationsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.notifications.delete_a_notification(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">update_a_notification</a>(...) -> AsyncHttpResponse[PatchNotificationsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.notifications.update_a_notification(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[PatchNotificationsIdRequestStatus]` — Notification status
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Update extended data
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Webhooks
<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">list_all_webhooks</a>(...) -> AsyncHttpResponse[GetWebhooksResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.list_all_webhooks()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">create_a_webhook</a>(...) -> AsyncHttpResponse[PostWebhooksResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.create_a_webhook(
    name="name",
    url="url",
    events=["events"],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` — Webhook name
    
</dd>
</dl>

<dl>
<dd>

**url:** `str` — Target URL
    
</dd>
</dl>

<dl>
<dd>

**events:** `typing.Sequence[str]` — List of event types (e.g. post.created)
    
</dd>
</dl>

<dl>
<dd>

**secret:** `typing.Optional[str]` — Secret for signature verification (auto-generated if missing)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">get_a_webhook</a>(...) -> AsyncHttpResponse[GetWebhooksIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.get_a_webhook(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">delete_a_webhook</a>(...) -> AsyncHttpResponse[DeleteWebhooksIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.delete_a_webhook(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">list_webhook_deliveries</a>(...) -> AsyncHttpResponse[GetWebhooksIdDeliveriesResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.list_webhook_deliveries(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Webhook ID
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Pagination cursor
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` — Items per page
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">get_a_delivery_from_webhook</a>(...) -> AsyncHttpResponse[GetWebhooksIdDeliveriesSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.get_a_delivery_from_webhook(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Webhook ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Delivery ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">delete_a_delivery_from_webhook</a>(...) -> AsyncHttpResponse[DeleteWebhooksIdDeliveriesSubIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.webhooks.delete_a_delivery_from_webhook(
    id="id",
    sub_id="subId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Webhook ID
    
</dd>
</dl>

<dl>
<dd>

**sub_id:** `str` — Delivery ID
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Integrations
<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">list_all_integrations</a>(...) -> AsyncHttpResponse[GetIntegrationsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.integrations.list_all_integrations()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">create_an_integration</a>(...) -> AsyncHttpResponse[PostIntegrationsResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.integrations.create_an_integration(
    type="type",
    config={"key": "value"},
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `str` — Integration type (e.g. slack, discord)
    
</dd>
</dl>

<dl>
<dd>

**config:** `typing.Dict[str, typing.Any]` — JSON configuration
    
</dd>
</dl>

<dl>
<dd>

**enabled:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">get_an_integration</a>(...) -> AsyncHttpResponse[GetIntegrationsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.integrations.get_an_integration(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">delete_an_integration</a>(...) -> AsyncHttpResponse[DeleteIntegrationsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.integrations.delete_an_integration(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">update_an_integration</a>(...) -> AsyncHttpResponse[PatchIntegrationsIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.integrations.update_an_integration(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` — Integration name
    
</dd>
</dl>

<dl>
<dd>

**config:** `typing.Optional[typing.Dict[str, typing.Any]]` — JSON configuration (merged with existing)
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` — Enable/disable integration
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## SsOs
<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">list_all_ss_os</a>(...) -> AsyncHttpResponse[GetSsoResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.ss_os.list_all_ss_os()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">create_an_sso</a>(...) -> AsyncHttpResponse[PostSsoResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.ss_os.create_an_sso(
    name="name",
    client_id="clientId",
    client_secret="clientSecret",
    issuer="issuer",
    authorization_endpoint="authorizationEndpoint",
    token_endpoint="tokenEndpoint",
    user_info_endpoint="userInfoEndpoint",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` — Provider name (e.g. Google)
    
</dd>
</dl>

<dl>
<dd>

**client_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**client_secret:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**issuer:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**authorization_endpoint:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**token_endpoint:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**user_info_endpoint:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">get_an_sso</a>(...) -> AsyncHttpResponse[GetSsoIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.ss_os.get_an_sso(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">delete_an_sso</a>(...) -> AsyncHttpResponse[DeleteSsoIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.ss_os.delete_an_sso(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">update_an_sso</a>(...) -> AsyncHttpResponse[PatchSsoIdResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.ss_os.update_an_sso(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` — Provider name
    
</dd>
</dl>

<dl>
<dd>

**domain:** `typing.Optional[str]` — Email domain to match
    
</dd>
</dl>

<dl>
<dd>

**client_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**client_secret:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issuer:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**authorization_endpoint:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**token_endpoint:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**user_info_endpoint:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` — Enable/disable provider
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

