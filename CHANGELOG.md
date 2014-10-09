# Changelog

## 2.4.0 - 2014-09-09
Change-Id is now part of event attribute comparison [pull 23](https://github.com/sonyxperiadev/gerrit-events/pull/23)

Added [Callable](http://docs.oracle.com/javase/6/docs/api/java/util/concurrent/Callable.html) versions of the send command jobs [pull 24](https://github.com/sonyxperiadev/gerrit-events/pull/24)

Fixed waiting for replication for DraftPublished and ChangeMerged events [pull 25](https://github.com/sonyxperiadev/gerrit-events/pull/25)

**WARNING:** this breaks binary compatibility with previous versions as it removed an interface implementation from DraftPublished,
and therefore should have bumped the major version. But it was an oversight in the original implementation and is more considered a bug-fix;
so only the minor version is bumped.

## 2.3.0 - 2014-08-27
Added createdOn and lastUpdated for Change and createdOn for PatchSet attributes [a154e14](https://github.com/sonyxperiadev/gerrit-events/commit/a154e14938f2982e4240e43f873d2c029e163a3e)

Added methods to AbstractSendCommandJob that throws exception on connection error for easier retrying
[pull 22](https://github.com/sonyxperiadev/gerrit-events/pull/22)

## 2.2.0 - 2014-08-12
Added CommentAdded::comment event attribute [pull 18](https://github.com/sonyxperiadev/gerrit-events/pull/18)

Expose exit code and stderr of ssh commands [pull 19](https://github.com/sonyxperiadev/gerrit-events/pull/19)

## 2.1.0 - 2014-06-16
Added ChangeKind to PatchSet _(introduced in Gerrit 2.10)_ [pull 17](https://github.com/sonyxperiadev/gerrit-events/pull/17)

## 2.0.1 - 2014-05-16
Added notify field to REST ReviewInput [pull 16](https://github.com/sonyxperiadev/gerrit-events/pull/16)

## 2.0.0 - 2014-04-25
Initial separated release. [a29ec0b](https://github.com/sonyxperiadev/gerrit-events/commit/a29ec0b1f54b040ba2bd265c6f5269380f812034)