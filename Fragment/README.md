#Fragment

###Fragment Template
Copy and place to your fragment.

```java
import android.os.Bundle;
import android.support.annotation.Nullable;
import android.support.v4.app.Fragment;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
/**
 * A simple {@link Fragment} subclass.
 * Change name "TemplateFragment" to you name fragment class.
 */
public class TemplateFragment extends Fragment {

    private final String TAG = "TemplateFragment";
    private View rootView;

    //Constructor newInstance
    public static TemplateFragment newInstance() {
        TemplateFragment fragment = new TemplateFragment();

        //Put any other arguments
        /*
        Bundle args = new Bundle(); //Argument
        args.putString("key","value");
        fragment.setArguments(args);
        */

        return fragment;
    }

    @Override
    public void onCreate(@Nullable Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        //Fragment will not be destroyed on configuration changes 
        //setRetainInstance(true);

        //Read from Arguments
        if (getArguments() != null) {
            Bundle args = getArguments();
        }
    }

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        rootView = inflater.inflate(R.layout.you_fragment_xml, container, false);

        //Code hear...

        return rootView;
    }

    @Override
    public void onActivityCreated(Bundle savedInstanceState) {
        super.onActivityCreated(savedInstanceState);
        if (savedInstanceState != null) {
            // Restore state hear

        }
    }

    @Override
    public void onSaveInstanceState(Bundle outState) {
        super.onSaveInstanceState(outState);
        // Save state hear
    }
}
```
