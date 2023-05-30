# The NobusGram API

## Documentazione delle API NobusWare x Instagram

Le API consentono agli sviluppatori di accedere a informazioni e dati relativi agli utenti e ai contenuti di Instagram. 

Di seguito sono elencate le API disponibili insieme ai relativi endpoint, parametri ed esempi di richieste.

## 1. GET USER PROFILE INFORMATIONS

Questa API restituisce le informazioni dell'utente in base al nome utente fornito.

**Endpoint:** `http://nobusware.it/api/getuserinfo.php`

**Parametri:**
- `username` (stringa, obbligatorio): Il nome utente dell'utente di cui si desidera ottenere le informazioni.

**Esempio di richiesta:**
```sh
GET /api/getuserinfo.php?username=laurenxburch
```


## 2. GET USER PROFILE POSTS

Questa API restituisce i post dell'utente in base al nome utente fornito.

**Endpoint:** `http://nobusware.it/api/getuserposts.php`

**Parametri:**
- `username` (stringa, obbligatorio): Il nome utente dell'utente di cui si desidera ottenere i post.

**Esempio di richiesta:**
```sh
GET /api/getuserposts.php?username=laurenxburch
```


## 3. GET USER FOLLOWERS LIST (Experimental)

Questa API restituisce i follower dell'utente in base al nome utente fornito.

**Endpoint:** `http://nobusware.it/api/getfollowers.php`

**Parametri:**
- `username` (stringa, obbligatorio): Il nome utente dell'utente di cui si desidera ottenere i follower.

**Esempio di richiesta:**
```sh
GET /api/getfollowers.php?username=laurenxburch
```


## 4. GET WHERE USER WAS TAGGED

Questa API restituisce i post dell'utente in base al nome utente fornito e ad un tag specificato.

**Endpoint:** `http://nobusware.it/api/getuserpoststag.php`

**Parametri:**
- `username` (stringa, obbligatorio): Il nome utente dell'utente di cui si desidera ottenere i post.

**Esempio di richiesta:**
```sh
GET /api/getuserpoststag.php?username=laurenxburch
```


## 5. GET CURRENT USER STORY

Questa API restituisce le storie dell'utente in base al nome utente fornito.

**Endpoint:** `http://nobusware.it/api/getuserstories.php`

**Parametri:**
- `username` (stringa, obbligatorio): Il nome utente dell'utente di cui si desidera ottenere le storie.

**Esempio di richiesta:**
```sh
GET /api/getuserstories.php?username=laurenxburch
```


## 6. GET POST COMMENTS BY ID AND SHORTCODE

Questa API restituisce i commenti di un post in base all'ID del post e al suo shortcode.

**Endpoint:** `http://nobusware.it/api/getpostscomment.php`

**Parametri:**
- `post_id` (stringa, obbligatoria): L'ID del post di cui si desidera ottenere i commenti.
- `shortcode` (stringa, obbligatoria): Lo shortcode del post.

**Esempio di richiesta:**
```sh
GET /api/getpostscomment.php?post_id=3065602285203889649&shortcode=CqLNQlANB3x
