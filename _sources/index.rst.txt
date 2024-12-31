.. pie_menu_editor_docs documentation master file, created by
   sphinx-quickstart on Tue Dec  3 03:15:22 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. image:: /_static/images/pme_logo.webp
   :alt: Pie Menu Editor Logo
   :align: center

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Welcome to PME Documentation
============================

The Pie Menu Editor (PME) is an add-on for Blender that allows users to create 
custom menus, dialogs, and various UI elements to streamline their workflow.
If you have any questions or need help, please visit the :ref:`Support & Community<support-community-index>` section.

.. note:: This is a placeholder document.


.. _feature-overview:
Feature Overview
================

.. raw:: html

   <div class="grid-container">
      <div class="feature-box">
         <a href="customization/editors/pie_menu_editor.html" class="feature-content">
               <h2 class="feature-title">Pie Menu Editor</h2>
               <p class="feature-description">Allows to create nested pie menus with 8+ buttons.</p>
         </a>
         <div class="feature-preview">
               <a href="https://www.youtube.com/watch?v=COW109EjBsU">
                  <img src="/_static/images/overview/overview_vid_pie.png" 
                        alt="Pie Menu Demo">
               </a>
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/regular_menu_editor.html" class="feature-content">
               <h2 class="feature-title">Regular Menu Editor</h2>
               <p class="feature-description">Allows to create multi-column menus which can be called by using the assigned hotkey or used as a sub-menu.</p>
         </a>
         <div class="feature-preview">
               <a href="https://www.youtube.com/watch?v=bvDADkqMLEw">
                  <img src="/_static/images/overview/overview_vid_menu.png" 
                        alt="Regular Menu Demo">
               </a>
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/popup_dialog_editor.html" class="feature-content">
               <h2 class="feature-title">Pop-up Dialog Editor</h2>
               <p class="feature-description">Allows to create a layout of widgets that can be displayed in pie menus, dialogs, panels or toolbars.</p>
         </a>
         <div class="feature-preview">
               <a href="https://www.youtube.com/watch?v=JdbmDSV9wIU">
                  <img src="/_static/images/overview/overview_vid_popup.png" 
                        alt="Popup Dialog Demo">
               </a>
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/sticky_key_editor.html" class="feature-content">
               <h2 class="feature-title">Sticky Key Editor</h2>
               <p class="feature-description">Hotkeys can be set to have different actions when pressed or released, which is useful for temporarily activating a tool or mode.</p>
         </a>
         <div class="feature-preview">
               <a href="https://www.youtube.com/watch?v=pcFOPWnHC7U">
                  <img src="/_static/images/overview/overview_vid_sticky.png" 
                        alt="Sticky Key Demo">
               </a>
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/stack_key_editor.html" class="feature-content">
               <h2 class="feature-title">Stack Key Editor</h2>
               <p class="feature-description">Allows to stack commands and cycle between them using the assigned hotkey.</p>
         </a>
         <div class="feature-preview">
               <img src="/_static/images/overview/overview_vid_stack.png" 
                     alt="Stack Key Demo">
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/macro_operator_editor.html" class="feature-content">
               <h2 class="feature-title">Macro Operator Editor</h2>
               <p class="feature-description">Allows to create new tools using existing Blender tools without coding.</p>
         </a>
         <div class="feature-preview">
               <img src="/_static/images/overview/overview_vid_macro.png" 
                     alt="Macro Operator Demo">
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/modal_operator_editor.html" class="feature-content">
               <h2 class="feature-title">Modal Operator Editor</h2>
               <p class="feature-description">Allows to create interactive tools.</p>
         </a>
         <div class="feature-preview">
               <img src="/_static/images/overview/overview_vid_modal.png" 
                     alt="Modal Operator Demo">
         </div>
      </div>

      <div class="feature-box">
         <a href="customization/editors/property_editor.html" class="feature-content">
               <h2 class="feature-title">Property Editor</h2>
               <p class="feature-description">Allows to create custom properties for objects, materials, and more.</p>
         </a>
         <div class="feature-preview">
               <img src="/_static/images/overview/overview_vid_property.png" 
                     alt="Property Editor Demo">
         </div>
      </div>
   </div>

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Documentation
=============

.. toctree::
   :maxdepth: 2
   :caption: Getting Started

   getting_started/about_pme
   getting_started/installation
   basic_usage/quick_tutorial

.. toctree::
   :maxdepth: 2
   :caption: Editors

   customization/editors/pie_menu_editor
   customization/editors/regular_menu_editor
   customization/editors/popup_dialog_editor
   customization/editors/sticky_key_editor
   customization/editors/stack_key_editor
   customization/editors/modal_operator_editor
   customization/editors/macro_operator_editor
   customization/editors/property_editor
   customization/editors/editor_common_elements

   customization/ui_customization
   customization/settings
   customization/custom_icon

.. toctree::
   :maxdepth: 2
   :caption: Reference

   reference/terminology
   reference/pme_scripting_reference/index
   scripting_guide/index

.. toctree::
   :maxdepth: 2
   :caption: Examples & Resources

   examples/basic
   examples/practical
   examples/script_collection
   examples/knowledge_base

.. toctree::
   :maxdepth: 2
   :caption: Support & Community

   support_community/faq
   support_community/known_issues
   support_community/get_support
   support_community/contribute_to_pme
   support_community/changelog
