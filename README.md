# Rails Directory Structure Guide

There is a default directory structure that __Ruby on Rails__ comes with. The Rails guides go in depth in explaining the folder structure, but does not talk about the extra folders that commonly get added in Rails Apps.

The goal of this guide is to be a central place to learn about __ALL__ the folders that are used in Rails apps, _not just the ones that come by default_. 

We will also go over explaining __RSpec__ folder structure and any additional folders.

## Directory Structure

- [app](#app)
	- [assets](#app_assets)
		- [config](#app_assets_config)
		- [images](#app_assets_images)
		- [javascripts](#app_assets_javascripts)
		- [stylesheets](#app_assets_stylesheets)
	- [channels](#app_channels)
	- [controllers](#app_controllers)
	- [helpers](#app_helpers)
	- [jobs](#app_jobs)
	- [mailers](#app_mailers)
	- [models](#app_models)
	- [views](#app_views)
- [bin](#bin)
- [config](#config)
	- [environments](#config_environments)
	- [initializers](#config_initializers)
	- [locales](#config_locales)
- [db](#db)
	- [migrate](#db_migrate)
- [lib](#lib)
	- [assets](#lib_assets)
	- [tasks](#lib_tasks)
- [log](#log)
- [public](#public)
- [test](#test)
	- [controllers](#test_controllers)
	- [fixtures](#test_fixtures)
	- [helpers](#test_helpers)
	- [integration](#test_integration)
	- [mailers](#test_mailers)
	- [models](#test_models)
- [spec](#spec)
	- [factories](#spec_factories)
	- [helpers](#spec_helpers)
	- [mailers](#spec_mailers)
	- [models](#spec_models)
	- [requests](#spec_requests)
	- [routing](#spec_routing)
	- [support](#spec_support)
	- [views](#spec_views)
- [tmp](#tmp)
	- [cache](#tmp_cache)
- [vendor](#vendor)
	- [assets](#vendor_assets)
		- [javascripts](#vendor_assets_javascripts)
		- [stylesheets](#vendor_assets_stylesheets)

### <a name="app"></a> app

It organizes your application components. It's got subdirectories that hold the views, controllers, models, and more that handle business logic.
