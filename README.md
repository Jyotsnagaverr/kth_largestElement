# kth_largestElement

 vector<int> kLargest(int arr[], int n, int k)
    {
        // code here
        vector<int> ans;
        priority_queue<int> pq(arr, arr + n);
        
        for(int i = 0; i < k; i++) {
            ans.push_back(pq.top());
            pq.pop();
        }
        
        return ans;
    }
