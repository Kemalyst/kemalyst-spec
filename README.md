# kemalyst-spec

Kemalyst helpers to Crystal's `spec` forked from spec-kemal.

## Installation

Add it to your `shard.yml`.

```yaml
name: your-kemalyst-app
version: 0.1.0

dependencies:
  kemalyst:
    github: drujensen/kemalyst
  kemalyst-spec:
    github: drujensen/kemalyst-spec
```

## Usage

Just require it before your files in your `spec/spec_helper.cr`

```crystal
require "kemalyst-spec"
```

```crystal
# spec/controllers/your-controller_spec.cr

describe "Your::Controller" do

  # You can use get,post,put,patch,delete to call the corresponding route.
  it "renders /" do
    get "/"
    response.body.should eq "Hello World!"
  end

end
```

This is a fork from spec-kemal and modified to work with kemalyst.

## Contributing

1. Fork it ( https://github.com/drujensen/spec-kemalyst/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

## Contributors

- [sdogruyol](https://github.com/sdogruyol) Sdogruyol - creator, maintainer
- [drujensen](https://github.com/drujensen) drujensen - modified
