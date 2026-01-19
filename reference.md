# Reference
## Auth
<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">register</a>(...) -> AsyncHttpResponse[RegisterResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a new user in your forum instance. Requires API key for instance identification. Returns a JWT token for subsequent authenticated requests.
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

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">login</a>(...) -> AsyncHttpResponse[LoginResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Authenticate an existing user. Requires API key for instance identification. Returns a JWT token for subsequent authenticated requests.
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

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">me</a>() -> AsyncHttpResponse[MeResponse]</code></summary>
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
client.auth.me()

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

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">forgot_password</a>(...) -> AsyncHttpResponse[ForgotPasswordResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Request a password reset email. Requires API key for instance identification.
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
client.auth.forgot_password(
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

<details><summary><code>client.auth.<a href="src/foru_ms_sdk/auth/client.py">reset_password</a>(...) -> AsyncHttpResponse[ResetPasswordResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reset password using a reset token. Requires API key for instance identification.
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

## Search
<details><summary><code>client.search.<a href="src/foru_ms_sdk/search/client.py">search</a>() -> AsyncHttpResponse[SearchSearchResponse]</code></summary>
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
client.search.search()

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

## Tags
<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">list</a>(...) -> AsyncHttpResponse[TagListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of tags. Use cursor for pagination.
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
client.tags.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search tags by name or description
    
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

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">create</a>(...) -> AsyncHttpResponse[TagResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new tag.
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
client.tags.create(
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

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">retrieve</a>(...) -> AsyncHttpResponse[TagResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a tag by ID or slug (if supported).
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
client.tags.retrieve(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a tag.
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
client.tags.delete(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">update</a>(...) -> AsyncHttpResponse[UpdateTagsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing tag. Only provided fields will be modified.
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
client.tags.update(
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

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">list_subscribers</a>(...) -> AsyncHttpResponse[TagSubscriberListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of subscribers for Tag.
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
client.tags.list_subscribers(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">retrieve_subscriber</a>(...) -> AsyncHttpResponse[RetrieveSubscriberTagsResponse]</code></summary>
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
client.tags.retrieve_subscriber(
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

<details><summary><code>client.tags.<a href="src/foru_ms_sdk/tags/client.py">delete_subscriber</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.tags.delete_subscriber(
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
<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list</a>(...) -> AsyncHttpResponse[ThreadListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of threads. Use cursor for pagination.
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
client.threads.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search term for title
    
</dd>
</dl>

<dl>
<dd>

**tag_id:** `typing.Optional[str]` — Filter by tag ID
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Filter by author ID
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[ListThreadsRequestSort]` — Sort criteria
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">create</a>(...) -> AsyncHttpResponse[ThreadResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new thread.
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
client.threads.create(
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

**poll:** `typing.Optional[CreateThreadsRequestPoll]` — Poll data
    
</dd>
</dl>

<dl>
<dd>

**locked:** `typing.Optional[bool]` — Lock thread on creation
    
</dd>
</dl>

<dl>
<dd>

**pinned:** `typing.Optional[bool]` — Pin thread on creation
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">retrieve</a>(...) -> AsyncHttpResponse[ThreadResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a thread by ID or slug (if supported).
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
client.threads.retrieve(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a thread.
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
client.threads.delete(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">update</a>(...) -> AsyncHttpResponse[UpdateThreadsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing thread. Only provided fields will be modified.
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
client.threads.update(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_posts</a>(...) -> AsyncHttpResponse[ThreadPostListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of posts for Thread.
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
client.threads.list_posts(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Filter posts by author ID
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[ListPostsThreadsRequestSort]` — Sort posts by creation time
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search within post body
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ListPostsThreadsRequestType]` — Filter by interaction type
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">retrieve_post</a>(...) -> AsyncHttpResponse[RetrievePostThreadsResponse]</code></summary>
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
client.threads.retrieve_post(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_post</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.threads.delete_post(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_reactions</a>(...) -> AsyncHttpResponse[ThreadReactionListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of reactions for Thread.
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
client.threads.list_reactions(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ListReactionsThreadsRequestType]` — Filter by reaction type
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">create_reaction</a>(...) -> AsyncHttpResponse[ThreadReactionResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a Reaction in Thread.
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
client.threads.create_reaction(
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

**type:** `CreateReactionThreadsRequestType` — Type of reaction
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_reaction</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.threads.delete_reaction(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">retrieve_reaction</a>(...) -> AsyncHttpResponse[RetrieveReactionThreadsResponse]</code></summary>
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
client.threads.retrieve_reaction(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">list_subscribers</a>(...) -> AsyncHttpResponse[ThreadSubscriberListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of subscribers for Thread.
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
client.threads.list_subscribers(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">retrieve_subscriber</a>(...) -> AsyncHttpResponse[RetrieveSubscriberThreadsResponse]</code></summary>
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
client.threads.retrieve_subscriber(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">delete_subscriber</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.threads.delete_subscriber(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">retrieve_poll</a>(...) -> AsyncHttpResponse[ThreadPollResponse]</code></summary>
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
client.threads.retrieve_poll(
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">create_poll</a>(...) -> AsyncHttpResponse[ThreadPollResponse]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from foru_ms_sdk import ForumClient
from foru_ms_sdk.threads import CreatePollThreadsRequestOptionsItem

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.threads.create_poll(
    id="id",
    title="title",
    options=[
        CreatePollThreadsRequestOptionsItem(
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

**options:** `typing.Sequence[CreatePollThreadsRequestOptionsItem]` — Poll options (2-20)
    
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

<details><summary><code>client.threads.<a href="src/foru_ms_sdk/threads/client.py">update_poll</a>(...) -> AsyncHttpResponse[ThreadPollResponse]</code></summary>
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
client.threads.update_poll(
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
<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">list</a>(...) -> AsyncHttpResponse[PostListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of posts. Use cursor for pagination.
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
client.posts.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Filter posts by author ID
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[ListPostsRequestSort]` — Sort posts by creation time
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search within post body
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ListPostsRequestType]` — Filter by interaction type
    
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">create</a>(...) -> AsyncHttpResponse[PostResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new post.
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
client.posts.create(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">retrieve</a>(...) -> AsyncHttpResponse[PostResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a post by ID or slug (if supported).
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
client.posts.retrieve(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a post.
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
client.posts.delete(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">update</a>(...) -> AsyncHttpResponse[UpdatePostsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing post. Only provided fields will be modified.
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
client.posts.update(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">list_reactions</a>(...) -> AsyncHttpResponse[PostReactionListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of reactions for Post.
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
client.posts.list_reactions(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ListReactionsPostsRequestType]` — Filter by reaction type
    
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">create_reaction</a>(...) -> AsyncHttpResponse[PostReactionResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a Reaction in Post.
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
client.posts.create_reaction(
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

**type:** `CreateReactionPostsRequestType` — Type of reaction
    
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">delete_reaction</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.posts.delete_reaction(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">retrieve_reaction</a>(...) -> AsyncHttpResponse[RetrieveReactionPostsResponse]</code></summary>
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
client.posts.retrieve_reaction(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">list_posts</a>(...) -> AsyncHttpResponse[PostPostListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of posts for Post.
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
client.posts.list_posts(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Filter posts by author ID
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[ListPostsPostsRequestSort]` — Sort posts by creation time
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search within post body
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ListPostsPostsRequestType]` — Filter by interaction type
    
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">retrieve_post</a>(...) -> AsyncHttpResponse[RetrievePostPostsResponse]</code></summary>
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
client.posts.retrieve_post(
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

<details><summary><code>client.posts.<a href="src/foru_ms_sdk/posts/client.py">delete_post</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.posts.delete_post(
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

## Private Messages
<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">list</a>(...) -> AsyncHttpResponse[PrivateMessageListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of private messages. Use cursor for pagination.
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
client.private_messages.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**query:** `typing.Optional[str]` — Search query (title or body)
    
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

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">create</a>(...) -> AsyncHttpResponse[PrivateMessageResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new private message.
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
client.private_messages.create(
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

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">retrieve</a>(...) -> AsyncHttpResponse[PrivateMessageResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a private message by ID or slug (if supported).
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
client.private_messages.retrieve(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a private message.
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
client.private_messages.delete(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">update</a>(...) -> AsyncHttpResponse[UpdatePrivateMessagesResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing private message. Only provided fields will be modified.
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
client.private_messages.update(
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

**body:** `typing.Optional[str]` — Message content
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[str]` — Message status (read, unread, archived)
    
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

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">list_replies</a>(...) -> AsyncHttpResponse[PrivateMessageReplyListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of replies for Private Message.
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
client.private_messages.list_replies(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
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

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">create_reply</a>(...) -> AsyncHttpResponse[PrivateMessageReplyResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a Reply in Private Message.
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
client.private_messages.create_reply(
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

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">retrieve_reply</a>(...) -> AsyncHttpResponse[RetrieveReplyPrivateMessagesResponse]</code></summary>
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
client.private_messages.retrieve_reply(
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

<details><summary><code>client.private_messages.<a href="src/foru_ms_sdk/private_messages/client.py">delete_reply</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.private_messages.delete_reply(
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
<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">list</a>(...) -> AsyncHttpResponse[UserListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of users. Use cursor for pagination.
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
client.users.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search by username or display name
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[ListUsersRequestSort]` — Sort by creation date
    
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">create</a>(...) -> AsyncHttpResponse[UserResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new user.
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
client.users.create(
    username="username",
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

**username:** `str` — Username (letters, numbers, underscores, hyphens)
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` — Email address
    
</dd>
</dl>

<dl>
<dd>

**password:** `typing.Optional[str]` — Password (min 8 chars)
    
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

**url:** `typing.Optional[str]` — Website URL
    
</dd>
</dl>

<dl>
<dd>

**roles:** `typing.Optional[typing.Sequence[str]]` — Role slugs to assign
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">retrieve</a>(...) -> AsyncHttpResponse[UserResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a user by ID or slug (if supported).
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
client.users.retrieve(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a user.
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
client.users.delete(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">update</a>(...) -> AsyncHttpResponse[UpdateUsersResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing user. Only provided fields will be modified.
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
client.users.update(
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">list_followers</a>(...) -> AsyncHttpResponse[UserFollowerListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of followers for User.
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
client.users.list_followers(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">retrieve_follower</a>(...) -> AsyncHttpResponse[RetrieveFollowerUsersResponse]</code></summary>
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
client.users.retrieve_follower(
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">delete_follower</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.users.delete_follower(
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">list_following</a>(...) -> AsyncHttpResponse[UserFollowingListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of following for User.
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
client.users.list_following(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">retrieve_following</a>(...) -> AsyncHttpResponse[RetrieveFollowingUsersResponse]</code></summary>
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
client.users.retrieve_following(
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

<details><summary><code>client.users.<a href="src/foru_ms_sdk/users/client.py">delete_following</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.users.delete_following(
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
<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">list</a>(...) -> AsyncHttpResponse[RoleListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of roles. Use cursor for pagination.
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
client.roles.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**search:** `typing.Optional[str]` — Search by name or slug
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[ListRolesRequestSort]` — Sort order
    
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

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">create</a>(...) -> AsyncHttpResponse[RoleResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new role.
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
client.roles.create(
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

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">retrieve</a>(...) -> AsyncHttpResponse[RoleResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a role by ID or slug (if supported).
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
client.roles.retrieve(
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

**id:** `str` — Role ID
    
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

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a role.
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
client.roles.delete(
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

**id:** `str` — Role ID
    
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

<details><summary><code>client.roles.<a href="src/foru_ms_sdk/roles/client.py">update</a>(...) -> AsyncHttpResponse[UpdateRolesResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing role. Only provided fields will be modified.
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
client.roles.update(
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

**id:** `str` — Role ID
    
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
<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">list</a>(...) -> AsyncHttpResponse[ReportListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of reports. Use cursor for pagination.
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
client.reports.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[str]` — Filter by status
    
</dd>
</dl>

<dl>
<dd>

**reporter_id:** `typing.Optional[str]` — Filter by reporter ID
    
</dd>
</dl>

<dl>
<dd>

**reported_id:** `typing.Optional[str]` — Filter by reported user ID
    
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

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">create</a>(...) -> AsyncHttpResponse[ReportResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new report.
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
client.reports.create(
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

**status:** `typing.Optional[str]` — Report status (default: pending)
    
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

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">retrieve</a>(...) -> AsyncHttpResponse[ReportResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a report by ID or slug (if supported).
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
client.reports.retrieve(
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

**id:** `str` — Report ID
    
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

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a report.
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
client.reports.delete(
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

**id:** `str` — Report ID
    
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

<details><summary><code>client.reports.<a href="src/foru_ms_sdk/reports/client.py">update</a>(...) -> AsyncHttpResponse[UpdateReportsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing report. Only provided fields will be modified.
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
client.reports.update(
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

**id:** `str` — Report ID
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[str]` — Report status (pending, reviewed, resolved, dismissed)
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` — Updated description or admin notes
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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
<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">list</a>(...) -> AsyncHttpResponse[NotificationListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of notifications. Use cursor for pagination.
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
client.notifications.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[ListNotificationsRequestStatus]` — Filter by notification status
    
</dd>
</dl>

<dl>
<dd>

**user_id:** `typing.Optional[str]` — Filter by recipient user ID (admin only)
    
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

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">create</a>(...) -> AsyncHttpResponse[NotificationResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new notification.
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
client.notifications.create(
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

**status:** `typing.Optional[CreateNotificationsRequestStatus]` — Initial notification status
    
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

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">retrieve</a>(...) -> AsyncHttpResponse[NotificationResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a notification by ID or slug (if supported).
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
client.notifications.retrieve(
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

**id:** `str` — Notification ID
    
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

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a notification.
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
client.notifications.delete(
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

**id:** `str` — Notification ID
    
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

<details><summary><code>client.notifications.<a href="src/foru_ms_sdk/notifications/client.py">update</a>(...) -> AsyncHttpResponse[UpdateNotificationsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing notification. Only provided fields will be modified.
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
client.notifications.update(
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

**id:** `str` — Notification ID
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[UpdateNotificationsRequestStatus]` — Notification status
    
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
<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">list</a>(...) -> AsyncHttpResponse[WebhookListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of webhooks. Use cursor for pagination.

**Requires feature: webhooks**
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
client.webhooks.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">create</a>(...) -> AsyncHttpResponse[WebhookResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new webhook.

**Requires feature: webhooks**
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
client.webhooks.create(
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

**active:** `typing.Optional[bool]` — Whether webhook is active
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">retrieve</a>(...) -> AsyncHttpResponse[WebhookResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a webhook by ID or slug (if supported).

**Requires feature: webhooks**
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
client.webhooks.retrieve(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete a webhook.

**Requires feature: webhooks**
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
client.webhooks.delete(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">update</a>(...) -> AsyncHttpResponse[UpdateWebhooksResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing webhook. Only provided fields will be modified.

**Requires feature: webhooks**
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
client.webhooks.update(
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

**name:** `typing.Optional[str]` — Webhook name
    
</dd>
</dl>

<dl>
<dd>

**url:** `typing.Optional[str]` — Target URL
    
</dd>
</dl>

<dl>
<dd>

**events:** `typing.Optional[typing.Sequence[str]]` — Event types to trigger on
    
</dd>
</dl>

<dl>
<dd>

**secret:** `typing.Optional[str]` — New secret
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` — Enable/disable webhook
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">list_deliveries</a>(...) -> AsyncHttpResponse[WebhookDeliveryListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of deliveries for Webhook.

**Requires feature: webhooks**
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
client.webhooks.list_deliveries(
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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
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

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">retrieve_delivery</a>(...) -> AsyncHttpResponse[RetrieveDeliveryWebhooksResponse]</code></summary>
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
client.webhooks.retrieve_delivery(
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

<details><summary><code>client.webhooks.<a href="src/foru_ms_sdk/webhooks/client.py">delete_delivery</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
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
client.webhooks.delete_delivery(
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
<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">list</a>(...) -> AsyncHttpResponse[IntegrationListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of integrations. Use cursor for pagination.

**Requires feature: integrations**
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
client.integrations.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">create</a>(...) -> AsyncHttpResponse[IntegrationResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an new integration.

**Requires feature: integrations**
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
client.integrations.create(
    type="type",
    name="name",
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

**type:** `str` — Integration type (e.g. SLACK, DISCORD)
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` — Integration name
    
</dd>
</dl>

<dl>
<dd>

**config:** `typing.Dict[str, typing.Any]` — JSON configuration
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` — Whether integration is active
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">retrieve</a>(...) -> AsyncHttpResponse[IntegrationResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve an integration by ID or slug (if supported).

**Requires feature: integrations**
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
client.integrations.retrieve(
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

**id:** `str` — Integration ID
    
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

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete an integration.

**Requires feature: integrations**
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
client.integrations.delete(
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

**id:** `str` — Integration ID
    
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

<details><summary><code>client.integrations.<a href="src/foru_ms_sdk/integrations/client.py">update</a>(...) -> AsyncHttpResponse[UpdateIntegrationsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing integration. Only provided fields will be modified.

**Requires feature: integrations**
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
client.integrations.update(
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

**id:** `str` — Integration ID
    
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

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

## SSOs
<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">list</a>(...) -> AsyncHttpResponse[SsoListResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve a paginated list of ssos. Use cursor for pagination.

**Requires feature: sso**
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
client.ss_os.list()

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

**limit:** `typing.Optional[int]` — Items per page (max 75)
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — Cursor for pagination
    
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

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">create</a>(...) -> AsyncHttpResponse[SsoResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an new sso.

**Requires feature: sso**
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
client.ss_os.create(
    provider="OKTA",
    domain="domain",
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

**provider:** `CreateSsOsRequestProvider` — SSO provider type
    
</dd>
</dl>

<dl>
<dd>

**domain:** `str` — Email domain to match (e.g. 'acme.com')
    
</dd>
</dl>

<dl>
<dd>

**config:** `typing.Dict[str, typing.Any]` — Provider configuration (clientId, issuer, etc.)
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` — Whether SSO is active
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">retrieve</a>(...) -> AsyncHttpResponse[SsoResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve an sso by ID or slug (if supported).

**Requires feature: sso**
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
client.ss_os.retrieve(
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

**id:** `str` — SSO ID
    
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

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">delete</a>(...) -> AsyncHttpResponse[SuccessResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete an sso.

**Requires feature: sso**
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
client.ss_os.delete(
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

**id:** `str` — SSO ID
    
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

<details><summary><code>client.ss_os.<a href="src/foru_ms_sdk/ss_os/client.py">update</a>(...) -> AsyncHttpResponse[UpdateSsOsResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing sso. Only provided fields will be modified.

**Requires feature: sso**
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
client.ss_os.update(
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

**id:** `str` — SSO ID
    
</dd>
</dl>

<dl>
<dd>

**provider:** `typing.Optional[UpdateSsOsRequestProvider]` — SSO provider type
    
</dd>
</dl>

<dl>
<dd>

**domain:** `typing.Optional[str]` — Email domain to match
    
</dd>
</dl>

<dl>
<dd>

**config:** `typing.Optional[typing.Dict[str, typing.Any]]` — Provider configuration
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` — Enable/disable provider
    
</dd>
</dl>

<dl>
<dd>

**extended_data:** `typing.Optional[typing.Dict[str, typing.Any]]` — Custom extended data
    
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

## Provisioning
<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">list</a>(...) -> AsyncHttpResponse[ListProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve all instances owned by the authenticated user. Use the `handle` query parameter to get a single instance with its API key.
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
client.provisioning.list(
    provisioning_key="x-provisioning-key",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `typing.Optional[str]` — Optional handle to get a single instance
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">create</a>(...) -> AsyncHttpResponse[CreateProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new forum instance. Returns the instance details including the API key for accessing the forum API.
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
client.provisioning.create(
    provisioning_key="x-provisioning-key",
    name="name",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` — Display name for the instance
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` — URL-friendly identifier (slug)
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">update</a>(...) -> AsyncHttpResponse[UpdateProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an instance's name or handle. The `handle` field identifies which instance to update.
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
client.provisioning.update(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` — Current handle to identify the instance
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` — New display name
    
</dd>
</dl>

<dl>
<dd>

**new_handle:** `typing.Optional[str]` — New URL-friendly identifier
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">delete</a>(...) -> AsyncHttpResponse[DeleteProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Permanently delete an instance. This action cannot be undone.
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
client.provisioning.delete(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` — Handle of the instance to delete
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">get_billing</a>(...) -> AsyncHttpResponse[GetBillingProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve billing and subscription information for an instance.
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
client.provisioning.get_billing(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">change_plan</a>(...) -> AsyncHttpResponse[ChangePlanProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change an instance's subscription plan. Returns a checkout URL for upgrades or a billing portal URL for downgrades.
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
client.provisioning.change_plan(
    provisioning_key="x-provisioning-key",
    handle="handle",
    plan="FREE",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**plan:** `UpgradeInstancePlan` — Target plan
    
</dd>
</dl>

<dl>
<dd>

**is_annual:** `typing.Optional[bool]` — Use annual billing (default: true)
    
</dd>
</dl>

<dl>
<dd>

**return_url:** `typing.Optional[str]` — URL to return to after checkout/portal
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">regenerate_api_key</a>(...) -> AsyncHttpResponse[RegenerateApiKeyProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate a new API key for the instance. The old key will be invalidated.
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
client.provisioning.regenerate_api_key(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">get_usage</a>(...) -> AsyncHttpResponse[GetUsageProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve usage statistics for an instance including API requests, storage, and content counts.
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
client.provisioning.get_usage(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">list_team</a>(...) -> AsyncHttpResponse[ListTeamProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve all team members for an instance.
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
client.provisioning.list_team(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">invite_team</a>(...) -> AsyncHttpResponse[InviteTeamProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Invite new team members to an instance.
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
from foru_ms_sdk.provisioning import InviteTeamProvisioningRequestMembersItem

client = ForumClient(
    api_key="YOUR_API_KEY",
)
client.provisioning.invite_team(
    provisioning_key="x-provisioning-key",
    handle="handle",
    members=[
        InviteTeamProvisioningRequestMembersItem(
            email="email",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**members:** `typing.Sequence[InviteTeamProvisioningRequestMembersItem]` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">remove_team_member</a>(...) -> AsyncHttpResponse[RemoveTeamMemberProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove a team member from an instance.
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
client.provisioning.remove_team_member(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `str` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">list_domains</a>(...) -> AsyncHttpResponse[ListDomainsProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve all custom domains for an instance.
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
client.provisioning.list_domains(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">add_domain</a>(...) -> AsyncHttpResponse[AddDomainProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Add a custom domain to an instance.
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
client.provisioning.add_domain(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` — Domain name (e.g., forum.example.com)
    
</dd>
</dl>

<dl>
<dd>

**subdomain:** `typing.Optional[str]` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">remove_domain</a>(...) -> AsyncHttpResponse[RemoveDomainProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove a custom domain from an instance.
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
client.provisioning.remove_domain(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">export_data</a>(...) -> AsyncHttpResponse[ExportDataProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Export all data from an instance including threads, posts, users, tags, etc.
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
client.provisioning.export_data(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">list_webhooks</a>(...) -> AsyncHttpResponse[ListWebhooksProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve all webhooks configured for an instance.
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
client.provisioning.list_webhooks(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">create_webhook</a>(...) -> AsyncHttpResponse[CreateWebhookProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new webhook for an instance.
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
client.provisioning.create_webhook(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**url:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**events:** `typing.Sequence[str]` 
    
</dd>
</dl>

<dl>
<dd>

**secret:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">update_webhook</a>(...) -> AsyncHttpResponse[UpdateWebhookProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update an existing webhook.
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
client.provisioning.update_webhook(
    provisioning_key="x-provisioning-key",
    handle="handle",
    webhook_id="webhookId",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**webhook_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**url:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**events:** `typing.Optional[typing.Sequence[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**secret:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**active:** `typing.Optional[bool]` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">delete_webhook</a>(...) -> AsyncHttpResponse[DeleteWebhookProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a webhook from an instance.
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
client.provisioning.delete_webhook(
    provisioning_key="x-provisioning-key",
    handle="handle",
    webhook_id="webhookId",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**webhook_id:** `str` 
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">get_ownership</a>(...) -> AsyncHttpResponse[GetOwnershipProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Retrieve owner and creator information for an instance.
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
client.provisioning.get_ownership(
    provisioning_key="x-provisioning-key",
    handle="handle",
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

**handle:** `str` — Instance handle
    
</dd>
</dl>

<dl>
<dd>

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">transfer_ownership</a>(...) -> AsyncHttpResponse[TransferOwnershipProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Transfer instance ownership to another user. Only the current owner can transfer ownership.
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
client.provisioning.transfer_ownership(
    provisioning_key="x-provisioning-key",
    handle="handle",
    new_owner_email="newOwnerEmail",
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

**provisioning_key:** `str` — User provisioning key for platform-level instance management
    
</dd>
</dl>

<dl>
<dd>

**handle:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**new_owner_email:** `str` — Email of the new owner
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">register</a>(...) -> AsyncHttpResponse[RegisterProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new account and receive a provisioning key for API access. Use this key to create and manage instances.
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
client.provisioning.register(
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

**email:** `str` — Email address for the account
    
</dd>
</dl>

<dl>
<dd>

**password:** `str` — Password (minimum 8 characters)
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` — Display name (optional)
    
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

<details><summary><code>client.provisioning.<a href="src/foru_ms_sdk/provisioning/client.py">login</a>(...) -> AsyncHttpResponse[LoginProvisioningResponse]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Login with email and password to retrieve your provisioning key.
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
client.provisioning.login(
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

**email:** `str` — Account email
    
</dd>
</dl>

<dl>
<dd>

**password:** `str` — Account password
    
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

