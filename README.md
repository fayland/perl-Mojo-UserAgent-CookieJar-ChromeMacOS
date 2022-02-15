# NAME

Mojo::UserAgent::CookieJar::ChromeMacOS - readonly Chrome(MacOSx) cookies for Mojo::UserAgent

# SYNOPSIS

    use Mojo::UserAgent;
    use Mojo::UserAgent::CookieJar::ChromeMacOS;

    my $ua = Mojo::UserAgent->new;
    $ua->cookie_jar(Mojo::UserAgent::CookieJar::ChromeMacOS->new);

    # For Linux
    Mojo::UserAgent::CookieJar::ChromeMacOS->new(
        file => '~/.config/google-chrome/Default/Cookies',
        pass => 'peanuts', # hardcode for Linux
    );

# DESCRIPTION

Mojo::UserAgent::CookieJar::ChromeMacOS tries to read the cookie from Chrome on MacOSx.

it would be useful when you need handle tricky logins or captchas.

# AUTHOR

Fayland Lam <fayland@gmail.com>

# COPYRIGHT

Copyright 2016- Fayland Lam

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO

[HTTP::Cookies::ChromeMacOS](https://metacpan.org/pod/HTTP%3A%3ACookies%3A%3AChromeMacOS)
