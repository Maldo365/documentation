========
Viva.com
========

Connecting a **Viva.com** :doc:`payment terminal <../terminals>`  allows you to offer a fluid
payment flow to your customers and ease the work of your cashiers.

.. note::
   Viva.com lets you turn your phone into a mobile card reader: `Tap On Phone
   <https://www.viva.com/en-gb/blog/tap-on-phone-turn-your-phone-into-a-mobile-card-reader>`_.

Configuration
=============

Start by creating your Viva.com account on `Viva.com's website <https://www.viva.com>`_.

Locate your Viva.com credentials
--------------------------------

When configuring Viva.com in Point of Sale, you need to use specific credentials that are
available in your Viva.com account. These credentials include your :ref:`Merchant ID
<viva_com/id-key>`, :ref:`API key <viva_com/id-key>`, :ref:`POS API credentials
<viva_com/pos-api>`, and :ref:`Terminal ID <viva_com/identifier>` number.

.. _viva_com/id-key:

Merchant ID and API key
~~~~~~~~~~~~~~~~~~~~~~~

Locate your `Merchant ID and API key following the Viva documentation
<https://developer.viva.com/getting-started/find-your-account-credentials/merchant-id-and-api-key/>`_.
Then, save the keys and paste them into the Odoo :guilabel:`Merchant ID` and :guilabel:`API Key`
fields :ref:`when creating the payment method <viva_com/method-creation>`.

.. image:: viva_com/access-cred.png
   :alt: merchant ID and API key fields

.. note::
   These credentials are used for APIs that authenticate with Basic Auth.

.. _viva_com/pos-api:

POS API credentials
~~~~~~~~~~~~~~~~~~~

Locate and generate your `POS API credentials following the Viva documentation
<https://developer.viva.com/getting-started/find-your-account-credentials/pos-apis-credentials/>`_.
Then, save the keys and paste them in the Odoo :guilabel:`Client secret` and :guilabel:`Client ID`
fields :ref:`when creating the payment method <viva_com/method-creation>`.

.. warning::
   These credentials are only displayed once. Ensure you keep a copy to secure them.

.. image:: viva_com/api-cred.png
   :alt: Client secret and client ID fields

.. note::
   These credentials are used for Android and iOS POS Activation requests, as well as the Cloud
   Terminal API.

.. _viva_com/identifier:

Terminal ID
~~~~~~~~~~~

Your terminal ID number is used to identify your terminal. To find it:

#. Go to your Viva.com account and select the relevant account.
#. Go to :menuselection:`Sales --> Physical payments --> Card terminals` in the navigation menu.

The terminal ID number is located under the :guilabel:`Terminal ID (TID)` column. Save it to paste
it into the :guilabel:`Terminal ID` field :ref:`when creating the payment method
<viva_com/method-creation>`.

.. image:: viva_com/terminal-id.png
   :alt: Viva terminal ID

.. _viva_com/method-creation:

Configure the payment method
----------------------------

#. :doc:`Activate the POS Viva.com module <../../../../general/apps_modules>` to enable the
   payment terminal.
#. :doc:`Create the related payment method <../../payment_methods>` by going to
   :menuselection:`Point of Sale --> Configuration --> Payment Methods` and clicking
   :guilabel:`New`.
#. Set the journal type as :guilabel:`Bank`.
#. Select :guilabel:`Viva.com` in the :guilabel:`Use a Payment Terminal` field.
#. Fill in the mandatory fields with your:

   - :ref:`Merchant ID and API key <viva_com/ID-key>`
   - :ref:`Client ID and Client secret <viva_com/pos-api>`
   - :ref:`Terminal ID <viva_com/identifier>`

#. Save the form and copy the generated webhook URL from the :guilabel:`Viva.com Webhook
   Endpoint` field. This URL is necessary :ref:`when configuring the webhook <viva_com/webhook>`.

.. image:: viva_com/create-method-viva-com.png
   :alt: payment method creation form
   :scale: 75%

.. _viva_com/webhook:

Configure the webhook
---------------------

Webhooks allow you to receive real-time notifications whenever a transaction occurs within your
Viva.com account. Set them up for `payment transactions following the Viva.com documentation
<https://developer.viva.com/webhooks-for-payments/transaction-payment-created/>`_.

.. seealso::
   `Setting up webhooks <https://developer.viva.com/webhooks-for-payments/#setting-up-webhooks>`_

Link the payment method to a POS
--------------------------------

You can select the payment method in your POS settings once the payment method is created. To do so,
go to the :ref:`POS' settings <configuration/settings>` and add the payment method under the
:guilabel:`Payment methods` field of the :guilabel:`Payment` section.
