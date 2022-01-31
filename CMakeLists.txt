# SPDX-License-Identifier: Apache-2.0
# Various cmake functions for Laird Connectivity modules and projects

# Adds a framework ID file to the auto-generation list
#
# @param `file` - target file to add
function(add_fwk_id_file file)
    set_property(GLOBAL APPEND PROPERTY FWK_ID_FILE_LIST ${file})
endfunction()

# Adds a framework msgcode file to the auto-generation list
#
# @param `file` - target file to add
function(add_fwk_msgcode_file file)
    set_property(GLOBAL APPEND PROPERTY FWK_MSG_FILE_LIST ${file})
endfunction()

# Adds a framework type file to the auto-generation list
#
# @param `file` - target file to add
function(add_fwk_type_file file)
    set_property(GLOBAL APPEND PROPERTY FWK_TYPE_FILE_LIST ${file})
endfunction()
