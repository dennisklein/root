# General pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_pretty_printing pretty_printing.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_array_interface array_interface.py)

# TDirectory and subclasses pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_tdirectory_attrsyntax tdirectory_attrsyntax.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_tdirectoryfile_attrsyntax_get tdirectoryfile_attrsyntax_get.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_tfile_attrsyntax_get_writeobject_open tfile_attrsyntax_get_writeobject_open.py)

# TTree and subclasses pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_ttree_branch_attr ttree_branch_attr.py
                    COPY_TO_BUILDDIR TreeHelper.h)
ROOT_ADD_PYUNITTEST(pyroot_pyz_ttree_iterable ttree_iterable.py
                    COPY_TO_BUILDDIR TreeHelper.h)
ROOT_ADD_PYUNITTEST(pyroot_pyz_ttree_setbranchaddress ttree_setbranchaddress.py
                    COPY_TO_BUILDDIR TreeHelper.h)
ROOT_ADD_PYUNITTEST(pyroot_pyz_ttree_branch ttree_branch.py
                    COPY_TO_BUILDDIR TreeHelper.h)

# TCollection and subclasses pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_tcollection_len tcollection_len.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_tcollection_listmethods tcollection_listmethods.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_tcollection_operators tcollection_operators.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_tcollection_iterable tcollection_iterable.py)

# TSeqCollection and subclasses pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_tseqcollection_itemaccess tseqcollection_itemaccess.py)
ROOT_ADD_PYUNITTEST(pyroot_pyz_tseqcollection_listmethods tseqcollection_listmethods.py)

# TArray and subclasses pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_tarray_len tarray_len.py)

# RVec and subclasses pythonizations
ROOT_ADD_PYUNITTEST(pyroot_pyz_rvec_asrvec rvec_asrvec.py)

# RooAbsCollection and subclasses pythonizations
if(ROOT_roofit_FOUND)
  ROOT_ADD_PYUNITTEST(pyroot_pyz_rooabscollection_len rooabscollection_len.py)
endif()
