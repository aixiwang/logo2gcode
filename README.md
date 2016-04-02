# logo2gcode
Inspired by https://github.com/rcpedersen/snap-to-gcode
A tool to convert LOGO script to CNC gcode

Sample LOGO code:
<pre><code>
penup
sety 100
seth -90
arc 180 100
home
sety -100
seth 90
arc 180 100
setxy 100 100
pendown
setxy 100 -100
penup
setxy -100 100
pendown
setxy -100 -100
penup
home

</code></pre>

Command to convert LOGO to gcode:
<pre><code>
python logo2gcode.py logo.txt gc.txt 5 -5 3 2
</code></pre>


Generated NC code:
<pre><code>
G21

G1 Z10.000 

G1 Y200.000 

G1 X-200.000 Y200.000 

G1 Z-10.000 

G1 X-199.910 Y205.999 

G1 X-199.640 Y211.993 

G1 X-199.191 Y217.976 

G1 X-198.562 Y223.942 

G1 X-197.754 Y229.888 

G1 X-196.769 Y235.806 

G1 X-195.606 Y241.692 

G1 X-194.268 Y247.541 

G1 X-192.754 Y253.346 

G1 X-191.067 Y259.104 

G1 X-189.208 Y264.809 

G1 X-187.179 Y270.455 

G1 X-184.982 Y276.038 

G1 X-182.618 Y281.552 

G1 X-180.089 Y286.993 

G1 X-177.399 Y292.356 

G1 X-174.549 Y297.635 

G1 X-171.542 Y302.827 

G1 X-168.380 Y307.926 

G1 X-165.067 Y312.928 

G1 X-161.606 Y317.829 

G1 X-157.998 Y322.623 

G1 X-154.249 Y327.307 

G1 X-150.361 Y331.877 

G1 X-146.338 Y336.328 

G1 X-142.183 Y340.656 

G1 X-137.900 Y344.857 

G1 X-133.493 Y348.929 

G1 X-128.965 Y352.866 

G1 X-124.322 Y356.665 

G1 X-119.567 Y360.324 

G1 X-114.704 Y363.838 

G1 X-109.738 Y367.205 

G1 X-104.673 Y370.422 

G1 X-99.514 Y373.485 

G1 X-94.266 Y376.392 

G1 X-88.932 Y379.140 

G1 X-83.519 Y381.727 

G1 X-78.030 Y384.150 

G1 X-72.472 Y386.408 

G1 X-66.848 Y388.498 

G1 X-61.163 Y390.418 

G1 X-55.424 Y392.167 

G1 X-49.635 Y393.743 

G1 X-43.801 Y395.145 

G1 X-37.928 Y396.371 

G1 X-32.021 Y397.420 

G1 X-26.085 Y398.292 

G1 X-20.125 Y398.985 

G1 X-14.147 Y399.499 

G1 X-8.157 Y399.834 

G1 X-2.159 Y399.988 

G1 X3.841 Y399.963 

G1 X9.837 Y399.758 

G1 X15.824 Y399.373 

G1 X21.797 Y398.809 

G1 X27.751 Y398.065 

G1 X33.679 Y397.144 

G1 X39.578 Y396.045 

G1 X45.440 Y394.770 

G1 X51.262 Y393.319 

G1 X57.038 Y391.694 

G1 X62.762 Y389.897 

G1 X68.430 Y387.929 

G1 X74.036 Y385.792 

G1 X79.576 Y383.488 

G1 X85.044 Y381.018 

G1 X90.435 Y378.386 

G1 X95.745 Y375.593 

G1 X100.969 Y372.642 

G1 X106.102 Y369.536 

G1 X111.140 Y366.277 

G1 X116.077 Y362.868 

G1 X120.910 Y359.313 

G1 X125.635 Y355.615 

G1 X130.246 Y351.776 

G1 X134.740 Y347.801 

G1 X139.113 Y343.693 

G1 X143.360 Y339.456 

G1 X147.479 Y335.093 

G1 X151.465 Y330.608 

G1 X155.314 Y326.006 

G1 X159.024 Y321.291 

G1 X162.590 Y316.466 

G1 X166.011 Y311.537 

G1 X169.282 Y306.507 

G1 X172.400 Y301.381 

G1 X175.364 Y296.165 

G1 X178.169 Y290.861 

G1 X180.814 Y285.476 

G1 X183.297 Y280.014 

G1 X185.615 Y274.480 

G1 X187.765 Y268.879 

G1 X189.747 Y263.216 

G1 X191.557 Y257.496 

G1 X193.196 Y251.724 

G1 X194.660 Y245.906 

G1 X195.950 Y240.046 

G1 X197.063 Y234.150 

G1 X197.999 Y228.224 

G1 X198.756 Y222.272 

G1 X199.335 Y216.300 

G1 X199.734 Y210.314 

G1 X199.953 Y204.318 

G1 Z10.000 

G1 X0.000 Y200.000 

G1 Y0.000 

G1 Y-200.000 

G1 X200.000 

G1 Z-10.000 

G1 X199.910 Y-205.999 

G1 X199.640 Y-211.993 

G1 X199.191 Y-217.976 

G1 X198.562 Y-223.942 

G1 X197.754 Y-229.888 

G1 X196.769 Y-235.806 

G1 X195.606 Y-241.692 

G1 X194.268 Y-247.541 

G1 X192.754 Y-253.346 

G1 X191.067 Y-259.104 

G1 X189.208 Y-264.809 

G1 X187.179 Y-270.455 

G1 X184.982 Y-276.038 

G1 X182.618 Y-281.552 

G1 X180.089 Y-286.993 

G1 X177.399 Y-292.356 

G1 X174.549 Y-297.635 

G1 X171.542 Y-302.827 

G1 X168.380 Y-307.926 

G1 X165.067 Y-312.928 

G1 X161.606 Y-317.829 

G1 X157.998 Y-322.623 

G1 X154.249 Y-327.307 

G1 X150.361 Y-331.877 

G1 X146.338 Y-336.328 

G1 X142.183 Y-340.656 

G1 X137.900 Y-344.857 

G1 X133.493 Y-348.929 

G1 X128.965 Y-352.866 

G1 X124.322 Y-356.665 

G1 X119.567 Y-360.324 

G1 X114.704 Y-363.838 

G1 X109.738 Y-367.205 

G1 X104.673 Y-370.422 

G1 X99.514 Y-373.485 

G1 X94.266 Y-376.392 

G1 X88.932 Y-379.140 

G1 X83.519 Y-381.727 

G1 X78.030 Y-384.150 

G1 X72.472 Y-386.408 

G1 X66.848 Y-388.498 

G1 X61.163 Y-390.418 

G1 X55.424 Y-392.167 

G1 X49.635 Y-393.743 

G1 X43.801 Y-395.145 

G1 X37.928 Y-396.371 

G1 X32.021 Y-397.420 

G1 X26.085 Y-398.292 

G1 X20.125 Y-398.985 

G1 X14.147 Y-399.499 

G1 X8.157 Y-399.834 

G1 X2.159 Y-399.988 

G1 X-3.841 Y-399.963 

G1 X-9.837 Y-399.758 

G1 X-15.824 Y-399.373 

G1 X-21.797 Y-398.809 

G1 X-27.751 Y-398.065 

G1 X-33.679 Y-397.144 

G1 X-39.578 Y-396.045 

G1 X-45.440 Y-394.770 

G1 X-51.262 Y-393.319 

G1 X-57.038 Y-391.694 

G1 X-62.762 Y-389.897 

G1 X-68.430 Y-387.929 

G1 X-74.036 Y-385.792 

G1 X-79.576 Y-383.488 

G1 X-85.044 Y-381.018 

G1 X-90.435 Y-378.386 

G1 X-95.745 Y-375.593 

G1 X-100.969 Y-372.642 

G1 X-106.102 Y-369.536 

G1 X-111.140 Y-366.277 

G1 X-116.077 Y-362.868 

G1 X-120.910 Y-359.313 

G1 X-125.635 Y-355.615 

G1 X-130.246 Y-351.776 

G1 X-134.740 Y-347.801 

G1 X-139.113 Y-343.693 

G1 X-143.360 Y-339.456 

G1 X-147.479 Y-335.093 

G1 X-151.465 Y-330.608 

G1 X-155.314 Y-326.006 

G1 X-159.024 Y-321.291 

G1 X-162.590 Y-316.466 

G1 X-166.011 Y-311.537 

G1 X-169.282 Y-306.507 

G1 X-172.400 Y-301.381 

G1 X-175.364 Y-296.165 

G1 X-178.169 Y-290.861 

G1 X-180.814 Y-285.476 

G1 X-183.297 Y-280.014 

G1 X-185.615 Y-274.480 

G1 X-187.765 Y-268.879 

G1 X-189.747 Y-263.216 

G1 X-191.557 Y-257.496 

G1 X-193.196 Y-251.724 

G1 X-194.660 Y-245.906 

G1 X-195.950 Y-240.046 

G1 X-197.063 Y-234.150 

G1 X-197.999 Y-228.224 

G1 X-198.756 Y-222.272 

G1 X-199.335 Y-216.300 

G1 X-199.734 Y-210.314 

G1 X-199.953 Y-204.318 

G1 Z10.000 

G1 X0.000 Y-200.000 

G1 X200.000 Y200.000 

G1 Z-10.000 

G1 Y-200.000 

G1 Z10.000 

G1 X-200.000 Y200.000 

G1 Z-10.000 

G1 Y-200.000 

G1 Z10.000 

G1 X0.000 Y0.000 

M0
</code></pre>