.. _glossary:

Glossary
========

Each project can have an assigned glossary for any language as a shorthand for storing
terminology. Consistency is more easily maintained this way.
Terms from the glossary containing words from the currently translated string can be
displayed in the sidebar.

Managing glossaries
-------------------

.. versionchanged:: 4.5

   Glossaries are now regular translation components and you can use all
   Weblate features on them — commenting, storing in a Git repository, or
   adding explanations.

Use any component as a glossary by turning on :ref:`component-is_glossary`.

An empty glossary for a given project is automatically created with the project.
Glossaries are shared among all components of the same project, and optionally
with other projects using :ref:`component-links` on the glossary component.

The glossary component looks like any other component in Weblate:

.. image:: /images/glossary-component.png

You can browse all glossary terms:

.. image:: /images/glossary-browse.png

Glossary terms
--------------

Glossary terms are translated the same way regular strings are. You can
toggle additional features using the :guilabel:`Tools` menu for each term.

.. image:: /images/glossary-tools.png

Not translatable terms
++++++++++++++++++++++

.. versionadded:: 4.5

Glossary terms which are read-only are not meant to be translated. You can use
this for names or other terms which should not change while translating. Such
terms are visually highlighted in the glossary sidebar.

The terms can be flagged using :guilabel:`Tools` ↓
:guilabel:`Mark as read-only`. In the background this toggles the ``read-only``
flag of the string.

.. seealso::

   :ref:`custom-checks`

.. _glossary-forbidden:

Forbidden translations
++++++++++++++++++++++

.. versionadded:: 4.5

You can flag certain glossary terms as forbidden, meaning ones _not_ to be used
for translations. Use this to clarify translation when some words are
ambiguous or could have unexpected meanings.

Terms can be flagged using :guilabel:`Tools` ↓
:guilabel:`Mark as forbidden translation`. In the background this toggles the ``forbidden``
flag of the string.

.. seealso::

   :ref:`custom-checks`

.. _glossary-terminology:

Terminology
+++++++++++

.. versionadded:: 4.5

Flagging certain glossary terms as terminology puts them in
all glossary languages. Use this to flag important terms which should be
translated consistently.

The terms can be flagged in the source language using :guilabel:`Tools` ↓
:guilabel:`Mark as terminology`. In the background this toggles the
``terminology`` flag of the string.

.. seealso::

   :ref:`custom-checks`

.. _glossary-variants:

Variants
++++++++

Variants are a generic way to group strings together. All term variants are
listed in the glossary sidebar when translating.

.. hint::

   You can use this to add abbreviations or shorter expressions for a term.

.. seealso::

   :ref:`variants`
