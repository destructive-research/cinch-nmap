# Nmap IRC front end  plugin

This plugin uses nmap port scanner to check on open/closed ports
on target hosts.

you need to have nmap installed!

## Installation
First install the gem by running:
    [sudo] gem install cinch-nmap

Then load it in your bot:
    require "cinch"
    require "cinch/plugins/nmap"

    bot = Cinch::Bot.new do
      configure do |c|
        # add all required options here
        c.plugins.plugins = [Cinch::Plugins::Nmap] # optionally add more plugins
      end
    end

    bot.start

## Commands
### !nmap  < ip >
Port scan a host

## Options
None.
