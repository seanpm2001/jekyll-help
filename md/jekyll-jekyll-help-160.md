# [Everything fell off the rails](https://github.com/jekyll/jekyll-help/issues/160)

> state: **closed** opened by: **** on: ****

I&#x27;ve been using Jekyll for quite some time on my computer with no issues. Then tonight when I tried to build my site, Jekyll just barfed on me. I don&#x27;t know what could have changed.

I am using RVM and Bundler.

&#x60;&#x60;&#x60;
$ jekyll build
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:6: warning: already initialized constant Psych::ClassLoader::BIG_DECIMAL
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:6: warning: previous definition of BIG_DECIMAL was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:7: warning: already initialized constant Psych::ClassLoader::COMPLEX
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:7: warning: previous definition of COMPLEX was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:8: warning: already initialized constant Psych::ClassLoader::DATE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:8: warning: previous definition of DATE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:9: warning: already initialized constant Psych::ClassLoader::DATE_TIME
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:9: warning: previous definition of DATE_TIME was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:10: warning: already initialized constant Psych::ClassLoader::EXCEPTION
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:10: warning: previous definition of EXCEPTION was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:11: warning: already initialized constant Psych::ClassLoader::OBJECT
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:11: warning: previous definition of OBJECT was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:12: warning: already initialized constant Psych::ClassLoader::PSYCH_OMAP
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:12: warning: previous definition of PSYCH_OMAP was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:13: warning: already initialized constant Psych::ClassLoader::PSYCH_SET
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:13: warning: previous definition of PSYCH_SET was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:14: warning: already initialized constant Psych::ClassLoader::RANGE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:14: warning: previous definition of RANGE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:15: warning: already initialized constant Psych::ClassLoader::RATIONAL
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:15: warning: previous definition of RATIONAL was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:16: warning: already initialized constant Psych::ClassLoader::REGEXP
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:16: warning: previous definition of REGEXP was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:17: warning: already initialized constant Psych::ClassLoader::STRUCT
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:17: warning: previous definition of STRUCT was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:18: warning: already initialized constant Psych::ClassLoader::SYMBOL
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:18: warning: previous definition of SYMBOL was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/class_loader.rb:64: warning: already initialized constant Psych::ClassLoader::CACHE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/class_loader.rb:64: warning: previous definition of CACHE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/scalar_scanner.rb:8: warning: already initialized constant Psych::ScalarScanner::TIME
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/scalar_scanner.rb:8: warning: previous definition of TIME was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/scalar_scanner.rb:11: warning: already initialized constant Psych::ScalarScanner::FLOAT
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/scalar_scanner.rb:11: warning: previous definition of FLOAT was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/scalar_scanner.rb:17: warning: already initialized constant Psych::ScalarScanner::INTEGER
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/scalar_scanner.rb:17: warning: previous definition of INTEGER was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/stream.rb:12: warning: already initialized constant Psych::Nodes::Stream::ANY
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/stream.rb:12: warning: previous definition of ANY was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/stream.rb:15: warning: already initialized constant Psych::Nodes::Stream::UTF8
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/stream.rb:15: warning: previous definition of UTF8 was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/stream.rb:18: warning: already initialized constant Psych::Nodes::Stream::UTF16LE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/stream.rb:18: warning: previous definition of UTF16LE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/stream.rb:21: warning: already initialized constant Psych::Nodes::Stream::UTF16BE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/stream.rb:21: warning: previous definition of UTF16BE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/sequence.rb:42: warning: already initialized constant Psych::Nodes::Sequence::ANY
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/sequence.rb:42: warning: previous definition of ANY was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/sequence.rb:45: warning: already initialized constant Psych::Nodes::Sequence::BLOCK
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/sequence.rb:45: warning: previous definition of BLOCK was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/sequence.rb:48: warning: already initialized constant Psych::Nodes::Sequence::FLOW
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/sequence.rb:48: warning: previous definition of FLOW was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/scalar.rb:9: warning: already initialized constant Psych::Nodes::Scalar::ANY
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/scalar.rb:9: warning: previous definition of ANY was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/scalar.rb:12: warning: already initialized constant Psych::Nodes::Scalar::PLAIN
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/scalar.rb:12: warning: previous definition of PLAIN was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/scalar.rb:15: warning: already initialized constant Psych::Nodes::Scalar::SINGLE_QUOTED
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/scalar.rb:15: warning: previous definition of SINGLE_QUOTED was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/scalar.rb:18: warning: already initialized constant Psych::Nodes::Scalar::DOUBLE_QUOTED
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/scalar.rb:18: warning: previous definition of DOUBLE_QUOTED was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/scalar.rb:21: warning: already initialized constant Psych::Nodes::Scalar::LITERAL
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/scalar.rb:21: warning: previous definition of LITERAL was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/scalar.rb:24: warning: already initialized constant Psych::Nodes::Scalar::FOLDED
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/scalar.rb:24: warning: previous definition of FOLDED was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/mapping.rb:16: warning: already initialized constant Psych::Nodes::Mapping::ANY
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/mapping.rb:16: warning: previous definition of ANY was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/mapping.rb:19: warning: already initialized constant Psych::Nodes::Mapping::BLOCK
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/mapping.rb:19: warning: previous definition of BLOCK was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/nodes/mapping.rb:22: warning: already initialized constant Psych::Nodes::Mapping::FLOW
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/nodes/mapping.rb:22: warning: previous definition of FLOW was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/visitors/visitor.rb:10: warning: already initialized constant Psych::Visitors::Visitor::DISPATCH
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/visitors/visitor.rb:10: warning: previous definition of DISPATCH was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/handler.rb:26: warning: already initialized constant Psych::Handler::OPTIONS
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/handler.rb:26: warning: previous definition of OPTIONS was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/handler.rb:29: warning: already initialized constant Psych::Handler::EVENTS
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/handler.rb:29: warning: previous definition of EVENTS was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/visitors/yaml_tree.rb:386: warning: already initialized constant Psych::Visitors::YAMLTree::NULL
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/visitors/yaml_tree.rb:416: warning: previous definition of NULL was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/visitors/yaml_tree.rb:387: warning: already initialized constant Psych::Visitors::YAMLTree::BINARY_RANGE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/visitors/yaml_tree.rb:417: warning: previous definition of BINARY_RANGE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/visitors/yaml_tree.rb:388: warning: already initialized constant Psych::Visitors::YAMLTree::WS_RANGE
~/.rvm/gems/ruby-2.1.2/gems/psych-2.0.6/lib/psych/visitors/yaml_tree.rb:418: warning: previous definition of WS_RANGE was here
~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/parser.rb:33:in &#x60;&lt;class:Parser&gt;&#x27;: superclass mismatch for class Mark (TypeError)
	from ~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/parser.rb:32:in &#x60;&lt;module:Psych&gt;&#x27;
	from ~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych/parser.rb:1:in &#x60;&lt;top (required)&gt;&#x27;
	from ~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych.rb:7:in &#x60;require&#x27;
	from ~/.rvm/rubies/ruby-2.1.2/lib/ruby/2.1.0/psych.rb:7:in &#x60;&lt;top (required)&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/safe_yaml-1.0.3/lib/safe_yaml/psych_handler.rb:1:in &#x60;require&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/safe_yaml-1.0.3/lib/safe_yaml/psych_handler.rb:1:in &#x60;&lt;top (required)&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/safe_yaml-1.0.3/lib/safe_yaml/load.rb:130:in &#x60;require&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/safe_yaml-1.0.3/lib/safe_yaml/load.rb:130:in &#x60;&lt;module:SafeYAML&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/safe_yaml-1.0.3/lib/safe_yaml/load.rb:26:in &#x60;&lt;top (required)&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/jekyll-2.4.0/lib/jekyll.rb:26:in &#x60;require&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/jekyll-2.4.0/lib/jekyll.rb:26:in &#x60;&lt;top (required)&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/jekyll-2.4.0/bin/jekyll:6:in &#x60;require&#x27;
	from ~/.rvm/gems/ruby-2.1.2/gems/jekyll-2.4.0/bin/jekyll:6:in &#x60;&lt;top (required)&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/bin/jekyll:23:in &#x60;load&#x27;
	from ~/.rvm/gems/ruby-2.1.2/bin/jekyll:23:in &#x60;&lt;main&gt;&#x27;
	from ~/.rvm/gems/ruby-2.1.2/bin/ruby_executable_hooks:15:in &#x60;eval&#x27;
	from ~/.rvm/gems/ruby-2.1.2/bin/ruby_executable_hooks:15:in &#x60;&lt;main&gt;&#x27;
&#x60;&#x60;&#x60;

**Update:** The problem is *jekyll-archives*.
jekyll/jekyll-archives#18

### Comments
