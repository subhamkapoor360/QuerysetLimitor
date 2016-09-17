# QuerysetLimitor

INSTALLATION:

pip install QuerysetLimitor

Description:
Gets a fixed no of rows(User specified) into memeory when iterating over querysets

USAGE:

from QuerysetLimitor.QuerysetLimitor import QuerysetLimitor
queryset = QuerysetLimitor(Table.objects.all(),MAX_OBJ_NUM(optional))

Now iterating over the queryset bring MAX_OBJ_NUM into memory and iterates over
it and then gets the next MAX_OBJ_NUM into memory and so on.

NOTES:

MAX_OBJ_NUM defaults to 100000 if not passed

MA_OBJ_NUM can be set from Project.settings file

By Initailizing the MA_OBJ_NUM variable in settings file.


