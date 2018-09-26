test

# Shopify App Examples

This repository is home to the code examples highlighted in various [Shopify API tutorials](https://help.shopify.com/api/tutorials). They are designed solely for the purpose of introducing new developers to the Shopify API. The example apps are written in [Sinatra](https://github.com/sinatra/sinatra), but the concepts presented will also apply to developers building applications in other languages such as Python, Node.js and PHP.

## Tutorial index

**1 Getting Started:** Building a public Shopify application ([tutorial](https://help.shopify.com/api/tutorials/building-public-app))

**2 Charging For Your App:** Adding billing to your app ([tutorial](https://help.shopify.com/api/tutorials/adding-billing-to-your-app/))

## Requirements

* [Ruby](https://www.ruby-lang.org/en/documentation/installation/) (sample apps were written with Ruby 2.2.1)
* [Bundler for Ruby](http://bundler.io/), a dependency manager
* [Shopify Partners account](https://accounts.shopify.com/signup)

## Credentials

Follow [this guide](https://help.shopify.com/api/getting-started/api-credentials) to obtain your public app credentials from your Shopify Partners account.

This example app uses a `.env` file to store app credentials. After cloning the repository, create a `.env` file in the root folder (`/example-ruby-app`) using the code snippet below. Then, copy the values of the _API Key_ and _API Secret_ from your partner dashboard, and use them as the values in `.env`.

```bash
API_KEY=YOUR_API_KEY
API_SECRET=YOUR_SECRET_KEY
```

`YOUR_API_KEY` and `YOUR_SECRET_KEY` are the values you must replace.

## App URL

This tutorial series uses [ngrok](https://ngrok.com/) to create a secure tunnel from the internet to your local machine. For each installment in the series, you will need to copy the `APP_URL` generated by ngrok to your `app.rb` file.  Additionally, the `APP_URL` needs to be added to the **App URLs** section of your public app settings. These procedures are covered in the [Building a public Shopify application](https://help.shopify.com/api/tutorials/building-public-app) tutorial.

## Running the app

```ruby
bundle install
ruby 01\ Getting\ Started/app.rb
```
