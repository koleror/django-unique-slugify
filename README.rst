Automatically create a unique slug for a model.

Note that you don't need to do obj.slug = ... since this method updates the instance's slug field directly. All you usually need is: unique_slugify(obj, obj.title)

A frequent usage pattern is to override the save method of a model and call unique_slugify before the super(...).save() call.
