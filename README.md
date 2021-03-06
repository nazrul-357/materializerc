# Materialize Roundcube
Materialize CSS skin for Roundcube, optimized for mobile view. See more Materializecss framework on <http://materializecss.com/>.

This repository consists of two important directories to run the materialized view for Roundcube; **skins** and **plugins**.

## Skins
This directory contains **materialize** skin which must be put in the **skins** directory of Roundcube. The **materialize** **skin** and the **plugin** must be enabled manually or, for the skin, set as default in Roundcube's config.

```php
...
$config['skin']='materialize';
```

## Plugin
This directory contains **materialize** plugin which must be put in the **plugins** directory of Roundcube. The **materialize** **skin** and the **plugin** must be enabled manually or, for the skin, set as default in Roundcube's config.

```php
...
$config['plugins'] = array(
	...  
	'materialize',	
);
```

## Important Notes
* Do not apply this skin on production without testing first
* Backup your existing Roundcube installation first
* Do not enable the skin from anything other than Roundcube's main `config.inc.php`
* To **disable the skin**, edit the Roundcube's main `config.ing.php`:
  * change `$config['skin']` to any skin other than `materialize`.
  * remove `materialize` from `$config['plugins']`.
