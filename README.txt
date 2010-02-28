moneta-namespace
	by Roger Jungemann (MIT License)
	http://github.com/thefifthcircuit/moneta-namespace
	
An API which exactly mirrors Moneta, but allows for different namespaces to be
defined, thereby allowing one store to be used for several applications
without key collisions.

Inspired by the redis-namespace library.

Usage:

  require 'moneta/namespace'
	require 'moneta/memory'
	
	store = Moneta::Memory.new
	s = Moneta::Namespace.new store, "app"
	s["hello"] = "world"
	
	puts s.moneta_store["app:hello"] #=> "world"
	
Requires the moneta gem.