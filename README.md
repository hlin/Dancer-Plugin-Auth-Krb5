# NAME

Dancer::Plugin::Auth::Krb5 - kerberos authentication for Dancer web apps

# VERSION

Version 0.01

#INSTALLATION

To install this module, run the following commands:

    perl Makefile.PL
    make
    make test
    make install

# SYNOPSIS

    use Dancer::Plugin::Auth::Krb5;

    my $auth = krb5_auth($username, $password);
    if ($auth->errors){
        # auth failed
    }else{
        # auth success
    }

# CONFIGURATION

    session: 'SessionEngine'
    plugins:
        Auth::Krb5:
            realm: 'REALM.DOMAIN.COM'

reference [Dancer::Session](http://search.cpan.org/perldoc?Dancer::Session) for 'SessionEngine'

# METHODS

    use Dancer::Plugin::Auth::Krb5;

    my $auth = krb5_auth($username, $password);

## user

    $auth->user;

return username

## errors

    $auth->errors;

return error message

## realm

    $auth->realm;

return realm

# AUTHOR

Hypo Lin, `<hlin@cpan.org>`

# BUGS

Please report any bugs or feature requests to `bug-dancer-plugin-auth-krb5 at rt.cpan.org`, or through
the web interface at [http://rt.cpan.org/NoAuth/ReportBug.html?Queue=Dancer-Plugin-Auth-Krb5](http://rt.cpan.org/NoAuth/ReportBug.html?Queue=Dancer-Plugin-Auth-Krb5).  I will be notified, and then you'll
automatically be notified of progress on your bug as I make changes.

# SUPPORT

You can find documentation for this module with the perldoc command.

    perldoc Dancer::Plugin::Auth::Krb5

You can also look for information at:

- RT: CPAN's request tracker (report bugs here)

[http://rt.cpan.org/NoAuth/Bugs.html?Dist=Dancer-Plugin-Auth-Krb5](http://rt.cpan.org/NoAuth/Bugs.html?Dist=Dancer-Plugin-Auth-Krb5)

- AnnoCPAN: Annotated CPAN documentation

[http://annocpan.org/dist/Dancer-Plugin-Auth-Krb5](http://annocpan.org/dist/Dancer-Plugin-Auth-Krb5)

- CPAN Ratings

[http://cpanratings.perl.org/d/Dancer-Plugin-Auth-Krb5](http://cpanratings.perl.org/d/Dancer-Plugin-Auth-Krb5)

- Search CPAN

[http://search.cpan.org/dist/Dancer-Plugin-Auth-Krb5/](http://search.cpan.org/dist/Dancer-Plugin-Auth-Krb5/)



# ACKNOWLEDGEMENTS


# LICENSE AND COPYRIGHT

Copyright 2012 Hypo Lin.

This program is free software; you can redistribute it and/or modify it
under the terms of either: the GNU General Public License as published
by the Free Software Foundation; or the Artistic License.

See http://dev.perl.org/licenses/ for more information.


