==========
Onboarding
==========

When a new employee is hired, it is important to have an onboarding procedure that can be followed.
This ensures that all important information is provided to the employee, all necessary equipment is
assigned to them, all necessary training is performed, and any other steps necessary for the
business are carried out.

Proper onboarding ensures that new employees are given all the information and tools needed for them
to be successful in their role, and ensures a smooth transition to their new job.

View onboarding plan
====================

Before onboarding can begin, it is recommended to check the default onboarding plan that comes
preconfigured with the **Employees** app. To view the current default plan, navigate to
:menuselection:`Employees app --> Configuration --> Activity Plan`.

The two default plans are :guilabel:`Offboarding` and :guilabel:`Onboarding`. Click
:guilabel:`Onboarding` to view the detailed onboarding plan form.

.. _onboarding/plan-form:

The plan form displays the following information:

- :guilabel:`Plan Name`: the specific name for the plan.
- :guilabel:`Model`: specifies where this plan can be used. In this case, in the **Employees** app.
- :guilabel:`Department`: if left blank (the default setting) this plan is available for all
  departments. The plan can be department-specific by selecting the department using the drop-down
  menu.
- :guilabel:`Activities To Create`: this tab lists all the steps that must be carried out in order
  to complete the onboarding plan. The steps appear in a list view, and each step displays the
  following information:

  - :guilabel:`Activity Type`: the specific activity for the step. The default options are :guilabel:`Email`,
    :guilabel:`Call`, :guilabel:`Meeting`, :guilabel:`To-Do`, or :guilabel:`Upload Document`. If the
    **Sign** app is installed, a :guilabel:`Request Signature` option is available.
  - :guilabel:`Summary`: a short description of the step.
  - :guilabel:`Assignment`: the person assigned to perform the activity. The default options are:
    :guilabel:`Ask at launch`, :guilabel:`Default user`, :guilabel:`Coach`, :guilabel:`Manager`, and
    :guilabel:`Employee`. If the **Fleet** app is installed, a :guilabel:`Fleet Manager` option is
    available.

    .. note::
       The selection for the :guilabel:`Assignment` role is in relation to the employee. If
       :guilabel:`Coach` is selected, the employee's coach is assigned to the activity.

       If :guilabel:`Default user` is selected, an :guilabel:`Assigned to` field appears. Using the
       drop-down menu, select the user who will always be assigned this activity.

  - :guilabel:`Assigned to`: this field remains blank unless :guilabel:`Default user` is selected
    for the :guilabel:`Assignment` field. If :guilabel:`Default user` is selected, this field is
    populated with the selected user.
  - :guilabel:`Document to sign`: the corresponding document requiring a signature.
  - :guilabel:`Interval`: the time when the activity is due.
  - :guilabel:`Unit`: the set time interval, either :guilabel:`days`, :guilabel:`weeks`, or
    :guilabel:`months`.
  - :guilabel:`Trigger`: how scheduling is determined for the activity. Options are either
    :guilabel:`Before Plan Date` or :guilabel:`After Plan Date`.

    .. example::
       A laptop must be set up and registered to a new employee the day before they start work. The
       person who performs this step should always be the IT Manager, Abby Jones.

       To configure this activity with these parameters, the :guilabel:`Activity Type` is set to
       :guilabel:`To-Do`, with a summary of :guilabel:`Assign Laptop`. The :guilabel:`Assignment`
       field is set to :guilabel:`Default user`, and the :guilabel:`Assigned to` field is set to
       :guilabel:`Abby Jones`. The :guilabel:`Interval` is :guilabel:`1`, and the :guilabel:`Unit`
       is set to :guilabel:`days`. The :guilabel:`Trigger` is :guilabel:`Before Plan Date`.

       .. image:: onboarding/activity-plan.png
          :alt: An activity configured to assign a laoptop the day before an employee starts work.

Onboarding plan steps
---------------------

The default :guilabel:`Onboarding` plan is minimal, with three default steps. All steps are
:guilabel:`To-Do` activities, and are scheduled for the day the onboarding plan is launched
(:guilabel:`0 days Before Plan Date`).

- :guilabel:`Setup IT Materials`: the manager must gather and configure all IT materials.
- :guilabel:`Plan Training`: the manager must plan the training for the new employee.
- :guilabel:`Training`: the new employee must complete the training planned by the manager.

.. image:: onboarding/onboarding.png
   :alt: The three default steps in the Onboarding plan.

Modify onboarding plan
======================

The default onboarding plan is minimal, so that modifications can be made to accommodate any
company's onboarding needs. Every company has different requirements, thus it is necessary to add
the required steps to the onboarding plan.

If the onboarding plan is universal, add or modify the default onboarding plan. If the onboarding
plan needed is only for a specific department, then a new plan should be created, specifically for
that department.

To modify the default plan, first navigate to :menuselection:`Employees app --> Configuration -->
Activity Plan`, then click on :guilabel:`Onboarding`.

To modify a step, click on the step and an :guilabel:`Open: Activities` pop-up window appears. Make
any desired modifications to the step, then click :guilabel:`Save` to accept the changes and close
the pop-up window.

To add a new step, click :guilabel:`Add a line` at the bottom of the listed activities in the
:guilabel:`Activities To Create` tab, and a blank :guilabel:`Create Activities` pop-up window
appears. Enter all the information in the pop-up window, then click :guilabel:`Save & Close` if
there are no their steps to add, or click :guilabel:`Save & New` if more steps are needed.

Configure all the desired steps for the onboarding plan.

Create onboarding plan
======================

For some companies, specific onboarding plans may be necessary for some departments. For these
cases, a new department-specific onboarding plan may be needed.

To create a new onboarding plan, first navigate to :menuselection:`Employees app -->
Configuration --> Activity Plan`. Click the :guilabel:`New` button in the upper-left corner, and a
blank plan form loads.

Enter all the :ref:`high-level information <onboarding/plan-form>` for the plan. If this plan is
specific to a department, ensure the :guilabel:`Department` field is populated.

Next, add the various steps for the plan by clicking :guilabel:`Add a line` at the bottom of the
listed activities in the :guilabel:`Activities To Create` tab, and a blank :guilabel:`Create
Activities` pop-up window appears. Enter all the information in the pop-up window, then click
:guilabel:`Save & Close` if there are no other steps to add, or click :guilabel:`Save & New` if more
steps are needed.

Configure all the desired steps for the onboarding plan.

.. example::
   A company specializing in the manufacturing and selling of outdoor metal furniture may have a
   large factory that produces the products, and a separate sales office. This company may have two
   separate onboarding plans, one for factory workers, and one for office workers.

   The onboarding plan for the factory workers is set for the :guilabel:`Manufacturing` department,
   and includes specialized tasks relating to factory jobs. These include gathering the new
   employees uniform and safety gear, assigning a safety course, emailing their team about the new
   hire, going over benefits, and more.

   .. image:: onboarding/factory-onboarding.png
      :alt: An onboarding plan configured for factory workers.

Launch onboarding plan
======================

After an employee has been hired, and their employee profile :ref:`is created
<recruitment/new-employee>`, click the :guilabel:`Launch Plan` button on the employee profile, and a
blank :guilabel:`Launch Plan` pop-up window loads.

Using the drop-down menu, select the desired onboarding plan in the :guilabel:`Plan` field. Then,
using the calendar selector, set a date in the :guilabel:`Plan Date` field. This is typically the
employee's first day, but any date can be selected.

The right-side of the :guilabel:`Launch Plan` pop-up window displays all the steps in the selected
plan, grouped by what was selected in the :guilabel:`Assignment` fields on the :ref:`plan form
<onboarding/plan-form>`.

Once the :guilabel:`Plan` and :guilabel:`Plan Date` fields are configured, click the
:guilabel:`Schedule` button, and Odoo schedules everything in the plan, according to their
respective due dates. All scheduled activities appear in the chatter of the employee profile.

.. image:: onboarding/onboarding-chatter.png
   :alt: All onboarding tasks scheduled in the chatter.
