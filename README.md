A subversion fixture based on Alpine, which creates a default repo, "repo" and allows
anonymous write access.

`docker run -p 3690:3690 tobyc/subversion`

`svn checkout svn://localhost/repo`

If you want to make the repository permanent, run it like this:

```
mkdir /srv/svn
docker run -p 3690:3690 -v /srv/svn:/svn tobyc/subversion
```
