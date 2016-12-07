# Doing it backwards

How do  we find where each point in the CMP should go in the final NMO corrected gather?
It's surprisingly difficult to find a description of the actual method of calculating amplitudes in NMO correction.
The only one I found is a paragraph from \cite{Yilmaz_2001} (http://wiki.seg.org/wiki/NMO_for_a_flat_reflector):


> "The idea is to find the amplitude value at A′ on the NMO-corrected gather from the  amplitude value at A on the original CMP gather. Given quantities \(t_0\), \(x\), and \(V_{NMO}\), compute t from equation (1). [...] The amplitude value at this time can be computed using the amplitudes at the neighboring integer sample values [...] This is done by an interpolation scheme that involves the four samples."

What it says is that the correct way is to do it backwards. 
Instead of mapping each point on the CMP to where it should be on the NMO, we want to take each point in the NMO and sample the amplitude from the corresponding point on the CMP gather.


Figure: Single trace from CMP (a) and corresponding single trace from NMO (b). Should be like the other figure but blank other traces. Include data as .- to highlight that they are discrete numbers. Include arrow from 1 point in (b) to (a). There will be no exact point in (a) so show the 4 points around and an interpolated curve. 