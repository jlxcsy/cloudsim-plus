.. java:import:: org.cloudbus.cloudsim.util MathUtil

.. java:import:: java.util Collections

.. java:import:: java.util LinkedList

.. java:import:: java.util List

VmUtilizationHistory
====================

.. java:package:: org.cloudbus.cloudsim.vms
   :noindex:

.. java:type:: public class VmUtilizationHistory implements UtilizationHistory

   Stores resource utilization data for a specific \ :java:ref:`Vm`\ .

   :author: Anton Beloglazov, Manoel Campos da Silva Filho

Fields
------
history
^^^^^^^

.. java:field:: public final List<Double> history
   :outertype: VmUtilizationHistory

   **See also:** :java:ref:`.getHistory()`

previousTime
^^^^^^^^^^^^

.. java:field:: public double previousTime
   :outertype: VmUtilizationHistory

   **See also:** :java:ref:`.getPreviousTime()`

Constructors
------------
VmUtilizationHistory
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public VmUtilizationHistory(Vm vm, boolean enabled)
   :outertype: VmUtilizationHistory

   Instantiates the class to store resource utilization history for a specific \ :java:ref:`Vm`\ .

   :param vm: the vm to instantiates the object to store utilization history
   :param enabled: true if the history must be enabled by default, enabling usage history to be collected and stored; false if it must be disabled to avoid storing any history, in order to reduce memory usage

VmUtilizationHistory
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public VmUtilizationHistory(Vm vm)
   :outertype: VmUtilizationHistory

Methods
-------
addUtilizationHistory
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void addUtilizationHistory(double time)
   :outertype: VmUtilizationHistory

disable
^^^^^^^

.. java:method:: @Override public void disable()
   :outertype: VmUtilizationHistory

enable
^^^^^^

.. java:method:: @Override public void enable()
   :outertype: VmUtilizationHistory

getHistory
^^^^^^^^^^

.. java:method:: @Override public List<Double> getHistory()
   :outertype: VmUtilizationHistory

getMaxHistoryEntries
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getMaxHistoryEntries()
   :outertype: VmUtilizationHistory

getPreviousTime
^^^^^^^^^^^^^^^

.. java:method:: @Override public double getPreviousTime()
   :outertype: VmUtilizationHistory

getUtilizationMad
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public double getUtilizationMad()
   :outertype: VmUtilizationHistory

getUtilizationMean
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public double getUtilizationMean()
   :outertype: VmUtilizationHistory

getUtilizationVariance
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public double getUtilizationVariance()
   :outertype: VmUtilizationHistory

isEnabled
^^^^^^^^^

.. java:method:: @Override public boolean isEnabled()
   :outertype: VmUtilizationHistory

setMaxHistoryEntries
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void setMaxHistoryEntries(int maxHistoryEntries)
   :outertype: VmUtilizationHistory

setPreviousTime
^^^^^^^^^^^^^^^

.. java:method:: @Override public void setPreviousTime(double previousTime)
   :outertype: VmUtilizationHistory

