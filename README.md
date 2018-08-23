# NAME

Task::BeLike::KWAKWA - Be more like KWAKWA!

# TASK CONTENTS

## Apps

### [App::Ack](https://metacpan.org/pod/App::Ack)

    # search Perl related files (.pl, .pm, .t)
    $ ack --perl foo

    # search Perl files except .t
    $ echo "--type-add=plpm=.pl,.pm" >> ~/.ackrc
    $ ack --plpm foo

### [App::ForkProve](https://metacpan.org/pod/App::ForkProve)

### [Module::Version](https://metacpan.org/pod/Module::Version) for `mversion`

    $ mversion Mojolicious
    7.61

## DateTime manipulation

### [DateTime::Format::ISO8601](https://metacpan.org/pod/DateTime::Format::ISO8601)

    my $dt = DateTime::Format::ISO8601->parse_datetime('2018-01-01T00:00:00Z');

## Debugging

### [Reply](https://metacpan.org/pod/Reply)

Install [Term::ReadLine::Gnu](https://metacpan.org/pod/Term::ReadLine::Gnu). You'll likely need `libreadline-dev` or
`readline-devel` to have actual readline support.

        # ~/.replyrc
    script_line1 = use strict
        script_line2 = use warnings
        script_line3 = use 5.024000

        [Interrupt]
        [FancyPrompt]
        [DataDumper]
        [Colors]
        [ReadLine]
        [Hints]
        [Packages]
        [LexicalPersistence]
        [ResultCache]
        [Autocomplete::Packages]
        [Autocomplete::Lexicals]
        [Autocomplete::Functions]
        [Autocomplete::Globals]
        [Autocomplete::Methods]
        [Autocomplete::Commands]

### [Pry](https://metacpan.org/pod/Pry)

## Filesystem

## [File::chdir](https://metacpan.org/pod/File::chdir) more sensible way to change directories

## Module management

### [Pod::Readme](https://metacpan.org/pod/Pod::Readme)

## Testing

Testing is hard to get right. Consider when writing tests which category the
test falls under and test and organise appropriately. Typically they can be
categorized as integration tests (how major parts of a system work together),
unit tests (exercising modules), functional/user acceptance tests (use case
scenarios, BDD).

Avoid using `if` statements. If your tests have branches, your tests need
tests.

### [Test::BDD::Cucumber](https://metacpan.org/pod/Test::BDD::Cucumber)

### [Test::MockTime](https://metacpan.org/pod/Test::MockTime)

### [Test::Mojo](https://metacpan.org/pod/Test::Mojo) can be used to test Dancer2 apps too.

### [Test2::Suite](https://metacpan.org/pod/Test2::Suite) use [Test2::V0](https://metacpan.org/pod/Test2::V0)

### [Test2::Tools::Exception](https://metacpan.org/pod/Test2::Tools::Exception)

## Web

### [Catalyst](https://metacpan.org/pod/Catalyst)

### [Dancer2](https://metacpan.org/pod/Dancer2)

### [Mojolicious](https://metacpan.org/pod/Mojolicious)

# AUTHOR

Paul Williams <kwakwa@cpan.org>

# COPYRIGHT

Copyright 2018- Paul Williams

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO

[Task::BeLike::DAGOLDEN](https://metacpan.org/pod/Task::BeLike::DAGOLDEN),
[Task::BeLike::RJBS](https://metacpan.org/pod/Task::BeLike::RJBS).
