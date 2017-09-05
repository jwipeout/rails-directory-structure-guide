# Rails Directory Structure Guide

There is a default directory structure that __Ruby on Rails__ comes with. The Rails guides go in depth in explaining the folder structure, but does not talk about the extra folders that commonly get added in Rails Apps.

The goal of this guide is to be a central place to learn about __ALL__ the folders that are used in Rails apps, _not just the ones that come by default (Marked with asterisk)_. 

We will also go over explaining __RSpec__ folder structure and any additional folders.

## Directory Structure

- [app](#app)
	- [assets](#app_assets)
	- [channels](#app_channels)
	- [controllers](#app_controllers)
	- [*decorators](#app_decorators)
	- [*forms](#app_forms)
	- [helpers](#app_helpers)
	- [jobs](#app_jobs)
	- [mailers](#app_mailers)
	- [models](#app_models)
	- [*performers](#app_performers)
	- [*presenters](#app_presenters)
	- [*services](#app_services)
	- [*use_cases](#app_use_cases)
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
- [vendor](#vendor)

---

### <a name="app"></a> app

It organizes your application components. It's got subdirectories that hold the views, controllers, models, and more that handle business logic.

### <a name="app_assets"></a> app/assets

Holds the assets for your application including images, stylesheets, and javascript.

### <a name="app_channels"></a> app/channels

Contains channels used to setup connections with [ActionCable](http://guides.rubyonrails.org/action_cable_overview.html#channels).

### <a name="app_controllers"></a> app/controllers

Contains app [controllers](http://guides.rubyonrails.org/action_controller_overview.html).

### <a name="app_decorators"></a> *app/decorators

App decorators is a design pattern to remove view methods from models. 

- [github](https://github.com/drapergem/draper) draper gem
- [article](https://medium.com/@dljerome/design-patterns-in-ruby-decorator-b7f2da4153b0) explanation of decorator pattern.
- [video](http://railscasts.com/episodes/286-draper) Railscast - using draper gem.
- [video](https://www.youtube.com/watch?v=bHpVdOzrvkE) RailsConf - decorators.

The [Draper Gem](https://github.com/drapergem/draper) is a popular choice to use to help with creating and using decorators.

### <a name="app_forms"></a> *app/forms

Form Object is a design pattern that encapsulates logic related to validating and persisting data. Using these can improve the way you implement complex forms.

- [article](https://www.sitepoint.com/7-design-patterns-to-refactor-mvc-components-in-rails/) about using form objects in rails.
- [video](http://railscasts.com/episodes/416-form-objects) Railscast - implementing form objects.


### <a name="app_helpers"></a> app/helpers

Contains app [helpers](http://guides.rubyonrails.org/action_view_overview.html#overview-of-helpers-provided-by-action-view).

### <a name="app_jobs"></a> app/jobs

Contains app [jobs](http://guides.rubyonrails.org/v4.2/active_job_basics.html).

### <a name="app_mailers"></a> app/mailers

Contains app [mailers](http://guides.rubyonrails.org/action_mailer_basics.html).

### <a name="app_models"></a> app/models

Contains app [models](http://guides.rubyonrails.org/active_record_basics.html).

### <a name="app_performers"></a> *app/performers

Performers is another design pattern to abstract view methods from the model using modules. 

- [github](https://github.com/jwipeout/performer-pattern) details on the _Performer Pattern_.

### <a name="app_presenters"></a> *app/presenters

Presenters is another design pattern to abstract view methods from the model using PORO. 

- [article](http://nithinbekal.com/posts/rails-presenters/) about using presenters in rails.
- [article](https://gist.github.com/somebox/5a7ebf56e3236372eec4) comparing presenters to decorators.
- [video](http://railscasts.com/episodes/287-presenters-from-scratch) Railscast - implementing a presenter.

### <a name="app_services"></a> *app/services

Contains app services. A service object implements the user’s interactions with the application. It contains business logic that describe the connections with your domain objects.

- [article](https://www.netguru.co/blog/service-objects-in-rails-will-help) about using services in rails.
- [video](http://railscasts.com/episodes/398-service-objects) Railscast - implementing a service.
- [video](https://vimeo.com/106759024) domain driven Rails

### <a name="app_use_cases"></a> *app/use_cases

Use Cases is pretty much the same thing as services. They are designed to break up non-trivial business logic. 

- [article](https://webuild.envato.com/blog/a-case-for-use-cases/) details on _use cases_.

- [video](https://www.youtube.com/watch?v=atFN0rReJfA) on her article above.

### <a name="app_views"></a> app/views

Contains app [views](http://guides.rubyonrails.org/layouts_and_rendering.html).

---

### <a name="bin"></a> bin

Contains the rails script that starts your app and can contain other scripts you use to setup, update, deploy or run your application.

---

### <a name="config"></a> config

Configure your application's routes, database, and more. This is covered in more detail in [Configuring Rails Applications](http://guides.rubyonrails.org/configuring.html).

---

### <a name="db"></a> db

Contains your current database schema, as well as the database migrations.

---

### <a name="lib"></a> lib

Extended modules for your application.

---

### <a name="log"></a> log

Application log files.

---

### <a name="public"></a> public

The only folder seen by the world as-is. Contains static files and compiled assets.

---

### <a name="test"></a> test

Unit tests, fixtures, and other test apparatus. These are covered in [Testing Rails Applications](http://guides.rubyonrails.org/testing.html).

---

### <a name="spec"></a> spec

Alternative to test directory using BDD. [Rspec](http://guides.rubyonrails.org/testing.html) allows you to write an alternative syntax to Test Unit that reads more like a specification than a test.

---

### <a name="tmp"></a> tmp

Temporary files (like cache and pid files).

---

### <a name="vendor"></a> vendor

A place for all third-party code. In a typical Rails application this includes vendored gems.


