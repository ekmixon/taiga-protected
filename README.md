# IMPORTANT NOTICE ABOUT UPCOMING TAIGA 6 RELEASE

Taiga6 is just around the corner. Please read [our pre-announcement](https://blog.taiga.io/taiga6-pre-announcement.html) so you know what's most important about our best release ever.

## Taiga Protected

taiga-protected is a service that implements token validation.

This project is a part of the system. The complete system is integrated by:

- nginx with specific configuration.

- taiga-protected service to validate tokens (this repository)

- [taiga-contrib-protected](https://github.com/taigaio/taiga-contrib-protected) plugin, an alternative storage system for taiga-back.

### Configuration

The server has 2 configuration options:

- `SECRET_KEY`. This is the shared secret used by the signer.

- `MAX_AGE` (optional). This is the expiration time in seconds.

Options could be set using environment variables or in a `.env` file.

## Vendoring

How to update vendored libraries.

.. code::

   pip install -t _vendor -r _vendor/vendor.txt --no-compile --no-deps
   rm -rf _vendor/*.dist-info/

## Documentation

Currently, we have authored three main documentation hubs:

- **[API](https://taigaio.github.io/taiga-doc/dist/api.html)**: Our API documentation and reference for developing from Taiga API.
- **[Documentation](https://taigaio.github.io/taiga-doc/dist/)**: If you need to install Taiga on your own server, this is the place to find some guides.
- **[Taiga Resources](https://resources.taiga.io)**: This page is intended to be the support reference page for the users.

## Bug reports

If you **find a bug** in Taiga you can always report it:

- in [Taiga issues](https://tree.taiga.io/project/taiga/issues). **This is the preferred way**
- in [Github issues](https://github.com/taigaio/taiga-protected/issues)
- send us a mail to support@taiga.io if is a bug related to [tree.taiga.io](https://tree.taiga.io)
- send us a mail to security@taiga.io if is a **security bug**.

One of our fellow Taiga developers will search, find and hunt it as soon as possible.

Please, before reporting a bug, write down how can we reproduce it, your operating system, your browser and version, and if it's possible, a screenshot. Sometimes it takes less time to fix a bug if the developer knows how to find it.

## Community

If you **need help to setup Taiga**, want to **talk about some cool enhancemnt** or you have **some questions**, please write us to our [mailing list](https://groups.google.com/d/forum/taigaio).

To subscribe for announcements of releases, important changes and so on, please follow [@taigaio](https://twitter.com/taigaio) on Twitter.

## Contribute to Taiga

There are many different ways to contribute to Taiga's platform, from patches, to documentation and UI enhancements, just find the one that best fits with your skills. Check out our detailed [contribution guide](https://resources.taiga.io/how-can-i-contribute)

## Code of Conduct

Help us keep the Taiga Community open and inclusive. Please read and follow our [Code of Conduct](https://github.com/taigaio/code-of-conduct/blob/master/CODE_OF_CONDUCT.md).

## License

Every code patch accepted in Taiga codebase is licensed under [AGPL v3.0](http://www.gnu.org/licenses/agpl-3.0.html). You must be careful to not include any code that can not be licensed under this license.

Please read carefully [our license](https://github.com/taigaio/taiga-back/blob/master/LICENSE) and ask us if you have any questions as well as the [Contribution policy](https://github.com/taigaio/taiga-back/blob/master/CONTRIBUTING.md).
